# Comparing `tmp/mistapi-0.41.1.tar.gz` & `tmp/mistapi-0.41.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.41.1.tar", last modified: Tue Jun 20 12:34:26 2023, max compression
+gzip compressed data, was "mistapi-0.41.2.tar", last modified: Tue Jun 20 13:34:53 2023, max compression
```

## Comparing `mistapi-0.41.1.tar` & `mistapi-0.41.2.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.164548 mistapi-0.41.1/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.41.1/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-20 12:34:26.164662 mistapi-0.41.1/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.41.1/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-20 12:34:05.000000 mistapi-0.41.1/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-20 12:34:26.165110 mistapi-0.41.1/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.045762 mistapi-0.41.1/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.071389 mistapi-0.41.1/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)     8951 2023-06-20 07:31:31.000000 mistapi-0.41.1/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2962 2023-02-21 11:06:36.000000 mistapi-0.41.1/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    21501 2023-06-19 15:16:16.000000 mistapi-0.41.1/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-20 12:34:05.000000 mistapi-0.41.1/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.41.1/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.074541 mistapi-0.41.1/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.41.1/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.41.1/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.41.1/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.074964 mistapi-0.41.1/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.075346 mistapi-0.41.1/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.081743 mistapi-0.41.1/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/other_device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.082134 mistapi-0.41.1/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.085529 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7257 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7693 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.086346 mistapi-0.41.1/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.086901 mistapi-0.41.1/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.088318 mistapi-0.41.1/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.088971 mistapi-0.41.1/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      999 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.089716 mistapi-0.41.1/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.095845 mistapi-0.41.1/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1746 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6037 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.138998 mistapi-0.41.1/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7670 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4813 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6148 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2348 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11558 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20369 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4863 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4921 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2996 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5098 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1910 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4805 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15544 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4669 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4923 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3026 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8805 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1933 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4772 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4876 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16846 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8845 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4839 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8322 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4823 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32619 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5508 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7068 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4592 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4868 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3602 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7620 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5953 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.139999 mistapi-0.41.1/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.140990 mistapi-0.41.1/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.143784 mistapi-0.41.1/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2974 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1884 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.163405 mistapi-0.41.1/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4848 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6197 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4710 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2360 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17510 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    59201 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5139 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8644 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15837 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5879 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5813 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20773 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    62170 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1727 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4684 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4734 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4886 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5356 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3890 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6960 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5340 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6002 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4650 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.164267 mistapi-0.41.1/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1087 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2023-06-20 12:34:06.000000 mistapi-0.41.1/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11952 2023-06-19 15:14:23.000000 mistapi-0.41.1/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 12:34:26.073686 mistapi-0.41.1/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-20 12:34:26.000000 mistapi-0.41.1/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-20 12:34:26.000000 mistapi-0.41.1/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-20 12:34:26.000000 mistapi-0.41.1/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-20 12:34:26.000000 mistapi-0.41.1/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-20 12:34:26.000000 mistapi-0.41.1/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.733090 mistapi-0.41.2/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.41.2/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-20 13:34:53.733227 mistapi-0.41.2/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.41.2/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-20 13:31:39.000000 mistapi-0.41.2/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-20 13:34:53.733731 mistapi-0.41.2/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.589919 mistapi-0.41.2/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.599361 mistapi-0.41.2/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9670 2023-06-20 13:11:19.000000 mistapi-0.41.2/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3008 2023-06-20 12:50:42.000000 mistapi-0.41.2/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    22464 2023-06-20 13:01:59.000000 mistapi-0.41.2/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2229 2023-02-13 15:54:52.000000 mistapi-0.41.2/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.602004 mistapi-0.41.2/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.41.2/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.41.2/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2029 2023-02-09 11:01:08.000000 mistapi-0.41.2/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.602501 mistapi-0.41.2/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.602950 mistapi-0.41.2/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.610774 mistapi-0.41.2/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/call_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/other_device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.611201 mistapi-0.41.2/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.614386 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7257 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7693 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.615274 mistapi-0.41.2/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.615948 mistapi-0.41.2/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.617725 mistapi-0.41.2/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.618330 mistapi-0.41.2/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      999 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.618955 mistapi-0.41.2/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.626310 mistapi-0.41.2/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1746 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6037 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.663330 mistapi-0.41.2/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7670 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4813 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6148 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2348 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11558 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20369 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4863 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4921 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2996 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5098 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1910 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4805 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15544 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4669 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4923 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3026 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8805 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1933 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4772 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4876 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16846 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8845 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4839 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8322 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4823 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32619 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5508 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7068 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4592 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4868 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3602 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7620 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5953 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.666508 mistapi-0.41.2/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.675921 mistapi-0.41.2/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.699841 mistapi-0.41.2/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2974 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1884 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.731685 mistapi-0.41.2/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4848 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6197 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4710 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2360 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17510 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    59201 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5139 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8644 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15837 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5879 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5813 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20773 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    62170 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1727 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4684 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4734 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4886 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5356 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3890 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6960 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5340 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6002 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4650 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.732796 mistapi-0.41.2/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1087 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2023-06-20 13:31:39.000000 mistapi-0.41.2/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11952 2023-06-20 13:02:07.000000 mistapi-0.41.2/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-20 13:34:53.601394 mistapi-0.41.2/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-20 13:34:53.000000 mistapi-0.41.2/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-20 13:34:53.000000 mistapi-0.41.2/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-20 13:34:53.000000 mistapi-0.41.2/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-20 13:34:53.000000 mistapi-0.41.2/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-20 13:34:53.000000 mistapi-0.41.2/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.41.1/LICENSE` & `mistapi-0.41.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/PKG-INFO` & `mistapi-0.41.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.41.1
+Version: 0.41.2
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.41.1/README.md` & `mistapi-0.41.2/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/pyproject.toml` & `mistapi-0.41.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.41.1"
+version = "0.41.2"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.41.1/src/mistapi/__api_request.py` & `mistapi-0.41.2/src/mistapi/__api_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         -----------
         :return APIResponse
         """
         try:
             url = self._url(uri) + self._gen_query(query)
             logger.info(f"apirequest:mist_get: sending request to {url}")
             resp = self._session.get(url)
+            logger.debug(f"apirequest:mist_get: request headers: {resp.request.headers}")
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'apirequest:mist_get: HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'apirequest:mist_get: HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'apirequest:mist_get: Other error occurred: {err}')  # Python 3.6
             logger.error("apirequest:mist_get: Exception occurred", exc_info=True)
@@ -100,14 +101,16 @@
             logger.info(f"apirequest:mist_post: sending request to {url}")
             headers = {'Content-Type': "application/json"}
             logger.debug(f"apirequest:mist_post: Request body: {body}")
             if type(body) == str:
                 resp = self._session.post(url, data=body, headers=headers)
             else: 
                 resp = self._session.post(url, json=body, headers=headers)
+            logger.debug(f"apirequest:mist_post: request headers: {resp.request.headers}")
+            logger.debug(f"apirequest:mist_post: request body: {resp.request.body}")
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'apirequest:mist_post: HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'apirequest:mist_post: HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'apirequest:mist_post: Other error occurred: {err}')  # Python 3.6
             logger.error("apirequest:mist_post: Exception occurred", exc_info=True)
@@ -132,14 +135,16 @@
             logger.info(f"apirequest:mist_put: sending request to {url}")
             headers = {'Content-Type': "application/json"}
             logger.debug(f"apirequest:mist_put: Request body: {body}")
             if type(body) == str:
                 resp = self._session.put(url, data=body, headers=headers)
             else: 
                 resp = self._session.put(url, json=body, headers=headers)
+            logger.debug(f"apirequest:mist_put: request headers: {resp.request.headers}")
+            logger.debug(f"apirequest:mist_put: request body: {resp.request.body}")
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'apirequest:mist_put: HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'apirequest:mist_put: HTTP error description: {resp.json()}')
         except Exception as err:
             logger.error(f'apirequest:mist_put: Other error occurred: {err}')  # Python 3.6
             logger.error("apirequest:mist_put: Exception occurred", exc_info=True)
@@ -158,14 +163,15 @@
         -----------
         :return APIResponse
         """
         try: 
             url = self._url(uri) + self._gen_query(query)
             logger.info(f"apirequest:mist_delete: sending request to {url}")
             resp = self._session.delete(url)
+            logger.debug(f"apirequest:mist_delete: request headers: {resp.request.headers}")
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'apirequest:mist_delete: HTTP error occurred: {http_err}')  # Python 3.6
         except Exception as err:
             logger.error(f'apirequest:mist_delete: Other error occurred: {err}')  # Python 3.6
             logger.error("apirequest:mist_delete: Exception occurred", exc_info=True)
         else: 
@@ -201,14 +207,16 @@
                             generated_multipart_form_data[key] = (os.path.basename(multipart_form_data[key]), f, 'application/octet-stream')                            
                         else:
                             generated_multipart_form_data[key] = (None, json.dumps(multipart_form_data[key]), 'application/json')
                     except:
                         logger.error(f"apirequest:mist_post_file: multipart_form_data: Unable to parse JSON object {key} with value {multipart_form_data[key]}")            
             logger.debug(f"apirequest:mist_post_file: final multipart_form_data: {generated_multipart_form_data}")
             resp = self._session.post(url, files=generated_multipart_form_data)
+            logger.debug(f"apirequest:mist_post_file: request headers: {resp.request.headers}")
+            logger.debug(f"apirequest:mist_post_file: request body: {resp.request.body}")
             if files:
                 for f in files:
                     f.close()
             resp.raise_for_status()
         except HTTPError as http_err:
             logger.error(f'apirequest:mist_post_file: HTTP error occurred: {http_err}')  # Python 3.6
             logger.error(f'apirequest:mist_post_file: HTTP error description: {resp.json()}')
```

### Comparing `mistapi-0.41.1/src/mistapi/__api_response.py` & `mistapi-0.41.2/src/mistapi/__api_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 This module manages API responses
 '''
 
 from requests import Response
-from mistapi.__logger import logger
-from mistapi.__logger import console
+from mistapi.__logger import logger, console
 
 class APIResponse:
     """
     Class used to pass API Responses
 
     PARAMS
     -----------
@@ -33,43 +32,43 @@
         self.raw_data=""
         self.data={}
         self.url=url
         self.next=None
         self.headers = response.headers
         self.status_code=response.status_code
 
-        logger.info(f"apiresponse:Response Status Code: {response.status_code}")
+        logger.info(f"apiresponse:__init__: response status code: {response.status_code}")
         console.debug(f"Response Status Code: {response.status_code}")
 
         try:
             self.raw_data = response.content
             self.data = response.json()
             self._check_next()
-            logger.debug(f"apiresponse:HTTP Response processed")
+            logger.debug(f"apiresponse:__init__: HTTP response processed")
             if self.status_code >= 400 or (type(self.data) == object and self.data.get("error")):
-                logger.error(f"apiresponse:Response: {response}")
+                logger.error(f"apiresponse:__init__: response = {response}")
                 console.debug(f"Response: {self.data}")
         except Exception as err:
-            logger.error(f"apiresponse:Unable to process HTTP Response: \r\n{err}")
+            logger.error(f"apiresponse:__init__: unable to process HTTP Response: \r\n{err}")
 
     def _check_next(self) -> None:
-        logger.debug(f"apiresponse:in  > _check_next")
+        logger.debug(f"apiresponse:_check_next")
         if "next" in self.data:
             self.next = self.data["next"]
-            logger.debug(f"apiresponse:set next to {self.next}")
+            logger.debug(f"apiresponse:_check_next: set next to {self.next}")
         else:
             total = self.headers.get("X-Page-Total")
             limit = self.headers.get("X-Page-Limit")
             page = self.headers.get("X-Page-Page")
             if total and limit and page:
                 try:
                     total=int(total)
                     limit=int(limit)
                     page=int(page)
                 except:
-                    logger.error(f"apiresponse:Unable to convert total({total})/limit({limit})/page({page}) to int")
+                    logger.error(f"apiresponse:_check_next: unable to convert total({total})/limit({limit})/page({page}) to int")
                     console.error(f"Unable to convert total({total})/limit({limit})/page({page}) to int")
                 if limit * page < total:
                     uri = f"/api/{self.url.split('/api/')[1]}"
                     self.next= uri.replace(f"page={page}", f"page={page+1}")
-                    logger.debug(f"apiresponse:set next to {self.next}")
+                    logger.debug(f"apiresponse:_check_next: set next to {self.next}")
```

### Comparing `mistapi-0.41.1/src/mistapi/__api_session.py` & `mistapi-0.41.2/src/mistapi/__api_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import os
 import sys
 import requests
 from dotenv import load_dotenv
 from pathlib import Path
 from getpass import getpass
 
-from mistapi.__logger import console
-from mistapi.__logger import logger
+from mistapi.__logger import logger, console
 from mistapi.__api_request import APIRequest
 from mistapi.__models.privilege import Privileges
 
 
 ###### GLOBALS ######
 clouds = [
     {"short": "Europe 01", "host": "api.eu.mist.com", "cookies_ext": ".eu"},
@@ -86,15 +85,15 @@
         self.last_name = ""
         self.via_sso = False
         self.tags = []
 
         self.privileges = Privileges([])
         self.session_expiry = ""
 
-        logger.debug("API Session initialized")
+        logger.debug("apisession:__init__: API Session initialized")
 
     def __str__(self):
         fields = [
             "email",
             "first_name",
             "last_name",
             "phone",
@@ -127,20 +126,20 @@
         if env_file:
             if env_file.startswith("~/"):
                 env_file = os.path.join(
                     os.path.expanduser("~"), env_file.replace("~/", "")
                 )
             env_file = os.path.abspath(env_file)
             console.debug(f"Loading settings from {env_file}")
-            logger.debug(f"apisession:Loading settings from {env_file}")
+            logger.debug(f"apisession:_load_env: loading settings from {env_file}")
             dotenv_path = Path(env_file)
             load_dotenv(dotenv_path=dotenv_path)
         else:
             console.debug("Loading settings from env file")
-            logger.debug(f"apisession:Loading settings from env file")
+            logger.debug(f"apisession:_load_env: loading settings from env file")
             load_dotenv()
 
         if os.getenv("MIST_HOST"):
             self.set_cloud(os.getenv("MIST_HOST"))
         if os.getenv("MIST_APITOKEN"):
             self.set_api_token(os.getenv("MIST_APITOKEN"))
         if os.getenv("MIST_USER"):
@@ -158,189 +157,193 @@
         """
         Set Mist Cloud to reach.
 
         PARAMS
         -----------
         :param str cloud_uri - Mist FQDN to reach ("api.mist.com", "api.eu.mist.com", ...)
         """
-        logger.debug(f"apisession:in  > set_cloud")
+        logger.debug(f"apisession:set_cloud")
         self._cloud_uri = None
         for cloud in clouds:
             if cloud["host"] == cloud_uri:
                 self._cloud_uri = cloud_uri
-                logger.debug(f"apisession:Mist Cloud configured to {self._cloud_uri}")
+                logger.debug(f"apisession:set_cloud: Mist Cloud configured to {self._cloud_uri}")
                 console.debug(f"Mist Cloud configured to {self._cloud_uri}")
         if not self._cloud_uri:
-            logger.error(f"apisession:{cloud_uri} is not valid")
+            logger.error(f"apisession:set_cloud: {cloud_uri} is not valid")
             console.error(f"{cloud_uri} is not valid")
 
     def get_cloud(self):
         """
         Return the Mist Cloud currently configured
         """
-        logger.debug(f"apisession:in  > get_cloud")
+        logger.debug(f"apisession:get_cloud: return {self._cloud_uri}")
         return self._cloud_uri
 
     def select_cloud(self) -> None:
         """
         Display a menu to select the Mist Cloud
         """
-        logger.debug(f"apisession:in  > select_cloud")
+        logger.debug(f"apisession:select_cloud")
         resp = "x"
         i = 0
         print()
         print(" Mist Cloud Selection ".center(80, "-"))
         print()
         for cloud in clouds:
             print(f"{i}) {cloud['short']} (host: {cloud['host']})")
             i += 1
 
         print()
         resp = input(f"Select a Cloud (0 to {i}, or q to exit): ")
+        logger.info(f"apisession:select_cloud: input is {resp}")
         if resp == "q":
             sys.exit(0)
         elif resp == "i":
             self._cloud_uri = "api.mistsys.com"
         else:
             try:
                 resp_num = int(resp)
                 if resp_num >= 0 and resp_num <= i:
+                    logger.info(f"apisession:select_cloud: Mist Cloud is {clouds[resp_num]['host']}")
                     self.set_cloud(clouds[resp_num]["host"])
                 else:
                     print(f"Please enter a number between 0 and {i}.")
+                    logger.error(f"apisession:select_cloud: {resp} is not a valid input")
                     self.select_cloud()
             except:
                 print("\r\nPlease enter a number.")
+                logger.error(f"apisession:select_cloud: {resp} is not a valid input")
                 self.select_cloud()
 
     ####################################
     # AUTH FUNCTIONS
     def set_email(self, email: str = None) -> None:
         """
         Set the user email
 
         PARAMS
         -----------
         :param str email    If no email provided, an interactive input will ask for it
         """
-        logger.debug(f"apisession:in  > set_email")
+        logger.debug(f"apisession:set_email")
         if email:
             self.email = email
         else:
             self.email = input("Login: ")
-        logger.debug(f"apisession:Email configured to {self.email}")
+        logger.info(f"apisession:set_email: email configured to {self.email}")
         console.debug(f"Email configured to {self.email}")
 
     def set_password(self, password: str = None) -> None:
         """
         Set the user password
 
         PARAMS
         -----------
         :param str password    If no password provided, an interactive input will ask for it
         """
-        logger.debug(f"apisession:in  > set_password")
+        logger.debug(f"apisession:set_password")
         if password:
             self._password = password
         else:
             self._password = getpass("Password: ")
-        logger.debug(f"apisession:Password configured")
+        logger.info(f"apisession:set_password: password configured")
         console.debug(f"Password configured")
 
     def set_api_token(self, apitoken: str):
         """
         Set Mist API Token
 
         PARAMS
         -----------
         :param str apitoken
         """
-        logger.debug(f"apisession:in  > set_api_token")
+        logger.debug(f"apisession:set_api_token")
         self._apitoken = apitoken
         self._session.headers.update({"Authorization": "Token " + self._apitoken})
-        logger.debug(f"apisession:API Token configured")
+        logger.info(f"apisession:set_api_token: API Token configured")
         console.debug(f"API Token configured")
 
     def _process_login(self):
         """
         Function to authenticate a user with login/password.
         Will create and store a session used by other requests.
         """
 
-        logger.debug(f"apisession:in  > _process_login")
+        logger.debug(f"apisession:_process_login")
         print()
         print(" Login/Pwd authentication ".center(80, "-"))
         print()
 
         self._session = requests.session()
         if not self.email:
             self.set_email()
         if not self._password:
             self.set_password()
 
-        logger.debug(f"apisession:Email/Password configured")
+        logger.debug(f"apisession:_process_login: email/password configured")
         uri = "/api/v1/login"
         body = {"email": self.email, "password": self._password}
         resp = self._session.post(self._url(uri), json=body)
         if resp.status_code == 200:
-            logger.info(f"apisession:Authentication successful!")
+            logger.info(f"apisession:_process_login: authentication successful!")
             console.info("Authentication successful!")
             self._set_authenticated(True)
         else:
             logger.error(
-                f"apisession:Authentication failed: {resp.json().get('detail')}"
+                f"apisession:_process_login: authentication failed: {resp.json().get('detail')}"
             )
             console.error(f"Authentication failed: {resp.json().get('detail')}\r\n")
             self.email = None
             self._password = None
-            logger.debug(
-                f"apisession:Email/Password cleaned up. Restarting authentication function"
+            logger.info(
+                f"apisession:_process_login: email/password cleaned up. Restarting authentication function"
             )
             self._process_login()
 
     def login(self):
         """
         Log in on the Mist Cloud.
         If information are missing to get connected, they will be requested
         during the process.
         If login/password is used, 2FA may be requests. Once authenticated,
         the HTTP session and CSRF Token will be stored and used during the
         future API requests.
         """
-        logger.debug(f"apisession:in  > login")
+        logger.debug(f"apisession:login")
         if self._authenticated:
-            logger.info(f"apisession:Already logged in...")
+            logger.warning(f"apisession:login: already logged in...")
             console.info("Already logged in...")
         else:
-            logger.debug(f"apisession:Not authenticated yet")
+            logger.debug(f"apisession:login: not authenticated yet")
             if not self._cloud_uri:
                 self.select_cloud()
             if self._apitoken:
                 self._set_authenticated(True)
             if not self._authenticated:
                 self._process_login()
             # if successfuly authenticated
             if self.get_authentication_status():
-                logger.info(f"apisession:Authenticated")
+                logger.info(f"apisession:login: authenticated")
                 self._getself()
 
     def logout(self):
         """
         Log out from the Mist Cloud.
         If login/password is used, the HTTP session is destroyed.
         """
-        logger.debug(f"apisession:in  > logout")
+        logger.debug(f"apisession:logout")
         if not self._authenticated:
-            logger.error(f"apisession:Not logged in...")
+            logger.error(f"apisession:logout: not logged in...")
             console.error("Not logged in...")
         else:
             uri = "/api/v1/logout"
             resp = self.mist_post(uri)
             if resp.status_code == 200:
-                logger.info(f"apisession:Mist Session closed")
+                logger.info(f"apisession:logout: Mist Session closed and cleaned up")
                 console.info("Logged out")
                 self._set_authenticated(False)
             else:
                 try:
                     console.error(resp.json()["detail"])
                 except:
                     console.error(resp.text)
@@ -353,89 +356,88 @@
         during the future API requests.
         If False, clear the CSRF Token and delete the HTTP session.
 
         PARAMS
         -----------
         :param bool authentication_status
         """
-        logger.debug(f"apisession:in  > _set_authenticated")
-        logger.debug(f"apisession:authentication_status is {authentication_status}")
+        logger.debug(f"apisession:_set_authenticated")
+        logger.debug(f"apisession:_set_authenticated: authentication_status is {authentication_status}")
         if authentication_status == True:
             self._authenticated = True
-            logger.info(f"apisession:Session is now Authenticated")
+            logger.info(f"apisession:_set_authenticated: session is now \"Authenticated\"")
             if not self._apitoken:
-                logger.debug(f"apisession:Processing HTTP cookies")
+                logger.info(f"apisession:_set_authenticated: processing HTTP cookies")
                 try:
                     cookies_ext = next(
                         item["cookies_ext"]
                         for item in clouds
                         if item["host"] == self._cloud_uri
                     )
-                    logger.info(f"apisession:HTTP session cookies extracted")
+                    logger.info(f"apisession:_set_authenticated: HTTP session cookies extracted")
                 except:
                     cookies_ext = ""
-                    logger.error(f"apisession:Unable to extract HTTP session cookies")
+                    logger.error(f"apisession:_set_authenticated: unable to extract HTTP session cookies")
                 self._csrftoken = self._session.cookies["csrftoken" + cookies_ext]
                 self._session.headers.update({"X-CSRFToken": self._csrftoken})
-                logger.info(f"apisession:CSRF Token stored")
+                logger.info(f"apisession:_set_authenticated: CSRF Token stored")
         elif authentication_status == False:
             self._authenticated = False
-            logger.info(f"apisession:Session is now Unauthenticated")
+            logger.info(f"apisession:_set_authenticated: session is now \"Unauthenticated\"")
             self._csrftoken = ""
             del self._session
             logger.info(
-                f"apisession:CSRFT Token is cleaned up and HTTP Session deleted"
+                f"apisession:_set_authenticated: CSRFT Token is cleaned up and HTTP Session deleted"
             )
 
     def get_authentication_status(self) -> bool:
         """
         RETURN
         -----------
         Return the authentication status.
         """
-        logger.debug(f"apisession:in  > get_authentication_status")
+        logger.debug(f"apisession:get_authentication_status: return {self._authenticated}")
         return self._authenticated
 
     def get_api_token(self):
         """
         Retrieve and display the User/Org API Tokens
         """
-        logger.debug(f"apisession:in  > list_api_token")
-        logger.info(f'apisession:Sending GET request to "/api/v1/self/apitokens"')
+        logger.info(f'apisession:get_api_token: Sending GET request to "/api/v1/self/apitokens"')
         resp = self.mist_get("/api/v1/self/apitokens")
         return resp
 
     def create_api_token(self, token_name: str = None):
         """
         Create a new API Token with the current account (user/org)
 
         PARAMS
         -----------
         :param str API token name (optional)
         """
-        logger.debug(f"apisession:in  > create_api_token")
+        logger.debug(f"apisession:create_api_token")
         if token_name:
             body = {"name": token_name}
         logger.info(
-            f'apisession:Sending POST request to "/api/v1/self/apitokens" with name "{token_name}"'
+            f'apisession:create_api_token: sending POST request to "/api/v1/self/apitokens" with name "{token_name}"'
         )
         resp = self.mist_post("/api/v1/self/apitokens", body=body)
         return resp
 
     def delete_api_token(self, token_id: str):
         """
         Delete an API Token based on its token_id
 
         PARAMS
         -----------
         :param str api token_id
         """
-        logger.debug(f"apisession:in  > delete_api_token")
+        logger.debug(f"apisession:delete_api_token")
         logger.info(
-            f'apisession:Sending DELETE request to "/api/v1/self/apitokens" with token_id "{token_id}"'
+            f'apisession:delete_api_token: sending DELETE request to "/api/v1/self/apitokens" with token_id "{token_id}"'
         )
         uri = f"https://{self._cloud_uri}/api/v1/self/apitokens/{token_id}"
         resp = self._session.delete(uri)
         return resp
 
     def _two_factor_authentication(self, two_factor: str) -> bool:
         """
@@ -446,78 +448,78 @@
         -----------
         :param str two_factor - 2FA code to send to the Mist Cloud
 
         RETURN
         -----------
         :return bool - True if authentication succeed, False otherwise
         """
-        logger.debug(f"apisession:in  > two_factor_authentication")
+        logger.debug(f"apisession:_two_factor_authentication")
         uri = "/api/v1/login"
         body = {
             "email": self.email,
             "password": self._password,
             "two_factor": two_factor,
         }
         resp = self._session.post(self._url(uri), json=body)
         if resp.status_code == 200:
-            logger.info(f"apisession:2FA authentication successed")
+            logger.info(f"apisession:: _two_factor_authentication2FA authentication successed")
             console.info("2FA authentication successed")
             self._set_authenticated(True)
             return True
         else:
             logger.error(
-                f"apisession:2FA authentication failed with error code: {resp.status_code}"
+                f"apisession:_two_factor_authentication: 2FA authentication failed with error code: {resp.status_code}"
             )
             console.error(
                 f"2FA authentication failed with error code: {resp.status_code}\r\n"
             )
             return False
 
     def _getself(self) -> None:
         """
         Retrieve information about the current user and store them in the current object.
         """
-        logger.debug(f"apisession:in  > getself")
+        logger.debug(f"apisession:_getself")
         uri = "/api/v1/self"
-        logger.info(f'apisession:Sending GET request to "{uri}"')
+        logger.info(f'apisession:_getself: sending GET request to "{uri}"')
         resp = self.mist_get(uri)
         if resp.data:
             # Deal with 2FA if needed
             if (
                 resp.data.get("two_factor_required") is True
                 and resp.data.get("two_factor_passed") is False
             ):
-                logger.info(f"apisession:2FA request by Mist Cloud")
+                logger.info(f"apisession:_getself: 2FA request by Mist Cloud")
                 two_factor_ok = False
                 while not two_factor_ok:
                     two_factor = input("Two Factor Authentication code required: ")
                     two_factor_ok = self._two_factor_authentication(two_factor)
                 self._getself()
             # Get details of the account
             else:
                 logger.info(
-                    f"apisession:Authentication Ok. Processing account privileges"
+                    f"apisession:_getself: authentication Ok. Processing account privileges"
                 )
                 for key, val in resp.data.items():
                     if key == "privileges":
                         self.privileges = Privileges(resp.data["privileges"])
                     if key == "tags":
                         for tag in resp.data["tags"]:
                             self.tags.append(tag)
                     else:
                         setattr(self, key, val)
                 print()
                 print(" Authenticated ".center(80, "-"))
                 print(f"\r\nWelcome {self.first_name} {self.last_name}!\r\n")
                 logger.info(
-                    f"apisession:Account used: {self.first_name} {self.last_name}"
+                    f"apisession:_getself: account used: {self.first_name} {self.last_name}"
                 )
                 return True
         else:
-            logger.error(f"apisession:Authentication not valid...")
+            logger.error(f"apisession:_getself: authentication not valid...")
             console.error("Authentication not valid...\r\n")
             resp = input(
                 f"Do you want to try with new credentials for {self._cloud_uri} (y/N)? "
                 % ()
             )
             if resp.lower() == "y":
                 self._process_login()
@@ -525,56 +527,56 @@
             else:
                 sys.exit(0)
 
     ####################################
     # PRIVILEGES
 
     def get_privilege_by_org_id(self, org_id: str):
-        logger.debug(f"apisession:in  > get_privilege_by_org_id")
+        logger.debug(f"apisession:get_privilege_by_org_id")
         org_priv = next(
             (priv for priv in self.privileges if priv.get("org_id") == org_id), None
         )
         if org_priv:
-            logger.info(f"apisession:org {org_id} privileges found in user info")
-            logger.debug(f"apisession:{org_priv}")
+            logger.info(f"apisession:get_privilege_by_org_id: org {org_id} privileges found in user info")
+            logger.debug(f"apisession:get_privilege_by_org_id: {org_priv}")
             return org_priv
         else:
             logger.warn(
-                f"apisession:Unable of find org {org_id} privileges in user data"
+                f"apisession:get_privilege_by_org_id: unable of find org {org_id} privileges in user data"
             )
             logger.info(
-                f"apisession:Trying to request org {org_id} info from the Cloud"
+                f"apisession:get_privilege_by_org_id: trying to request org {org_id} info from the Cloud"
             )
             uri = f"/api/v1/orgs/{org_id}"
             msp_id = None
             try:
                 resp = self.mist_get(uri)
                 if resp.data and resp.data.get("msp_id"):
                     logger.info(
-                        f"apisession:org {org_id} belong to msp_id {resp.data['msp_id']}"
+                        f"apisession:get_privilege_by_org_id: org {org_id} belong to msp_id {resp.data['msp_id']}"
                     )
                     msp_id = resp.data.get("msp_id")
                 else:
                     logger.warn(
-                        "apisession: Not able to find msp_id information in the org info"
+                        "apisession:get_privilege_by_org_id: not able to find msp_id information in the org info"
                     )
             except:
-                logger.error("apisession:Error when retrieving org info")
+                logger.error("apisession:get_privilege_by_org_id: error when retrieving org info")
             if msp_id:
                 msp_priv = next(
                     (
                         priv
                         for priv in self.privileges
                         if priv.get("scope") == "msp" and priv.get("msp_id") == msp_id
                     ),
                     None,
                 )
                 if not msp_priv:
                     logger.warn(
-                        f"apisession:Unable of find msp {msp_id} privileges in user data"
+                        f"apisession:get_privilege_by_org_id: unable of find msp {msp_id} privileges in user data"
                     )
                     return None
                 else:
                     return {
                         "scope": "org",
                         "org_id": org_id,
                         "name": resp.data.get("name"),
```

### Comparing `mistapi-0.41.1/src/mistapi/__logger.py` & `mistapi-0.41.2/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/__models/privilege.py` & `mistapi-0.41.2/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/__pagination.py` & `mistapi-0.41.2/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listAlarmDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listAlarmDefinitions")  
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/applications.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/call_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listCallEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listCallEventsDefinitions")  
 def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listClientEventsDefinitions")  
-def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMxEdgeEventsDefinitions")  
+def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/client_events"
+    uri = f"/api/v1/const/mxedge_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/client_events"
+    uri = f"/api/v1/const/mxedge_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/countries.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/device_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listDeviceModels")  
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInsightMetrics")  
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/languages.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/languages.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMxEdgeEventsDefinitions")  
-def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listTrafficTypes")  
+def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/mxedge_events"
+    uri = f"/api/v1/const/traffic_types"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/mxedge_events"
+    uri = f"/api/v1/const/traffic_types"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/other_device_events.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/other_device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOtherDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOtherDeviceEventsDefinitions")  
 def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/two_factor.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,46 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listTrafficTypes")  
-def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
+def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
+    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    QUERY PARAMS
+    ------------
+    by : str{'qrcode'}, default: qrcode        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/traffic_types"
-    query_params={}
+    uri = f"/api/v1/self/two_factor/token"
+    query_params={}
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listTrafficTypes(mist_session:_APISession) -> _APIResponse:
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/traffic_types"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/two_factor/verify"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -85,15 +85,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.41.2/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.41.2/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/login/login.py` & `mistapi-0.41.2/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.41.2/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.41.2/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.41.2/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.41.2/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.41.2/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/licenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/search.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.41.2/src/mistapi/api/v1/msps/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -84,15 +84,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -316,15 +316,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -456,15 +456,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -157,15 +157,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -185,15 +185,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/pma.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/psks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgSsrUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgSsrUpgrades")  
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -255,15 +255,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -356,15 +356,15 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgsVpns")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgsVpns")  
 def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.41.2/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.41.2/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.41.2/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/register/register.py` & `mistapi-0.41.2/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/register/verify.py` & `mistapi-0.41.2/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/logs.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/self.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.41.2/src/mistapi/api/v1/const/client_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,54 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listClientEventsDefinitions")  
+def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
+    API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    by : str{'qrcode'}, default: qrcode        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
+    uri = f"/api/v1/const/client_events"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+def listClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
+    API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/two_factor/verify"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/const/client_events"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/self/update.py` & `mistapi-0.41.2/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteApps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteApps")  
 def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/beacons.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/call.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/count.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteDeviceProfilesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteDeviceProfilesDerived")  
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -745,15 +745,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/events.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -167,15 +167,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/location.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteNetworksDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteNetworksDerived")  
 def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/services.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteServicesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteServicesDerived")  
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/sites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -266,15 +266,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -469,15 +469,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWirelessClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWirelessClientsStats")  
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -555,15 +555,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -672,15 +672,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1045,15 +1045,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1094,15 +1094,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1725,15 +1725,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/uisettings.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/vpns.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/vpns.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteVpnsDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteVpnsDerived")  
 def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wan_client.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWxRules")  
 def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteWxTunnels")  
 def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.41.2/src/mistapi/api/v1/sites/zones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.1", details="function replaced with listSiteZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.2", details="function replaced with listSiteZones")  
 def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.41.2/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.41.2/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi/cli.py` & `mistapi-0.41.2/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.1/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.41.2/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.41.1
+Version: 0.41.2
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.41.1/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.41.2/src/mistapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

