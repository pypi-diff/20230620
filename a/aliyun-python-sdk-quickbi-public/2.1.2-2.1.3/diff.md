# Comparing `tmp/aliyun-python-sdk-quickbi-public-2.1.2.tar.gz` & `tmp/aliyun-python-sdk-quickbi-public-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-quickbi-public-2.1.2.tar", last modified: Thu May 11 02:50:51 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-quickbi-public-2.1.3.tar", last modified: Tue Jun 20 12:30:57 2023, max compression
```

## Comparing `aliyun-python-sdk-quickbi-public-2.1.2.tar` & `aliyun-python-sdk-quickbi-public-2.1.3.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6470 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1552 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1403 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1226 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1934 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6770 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryComponentPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryCubeOptimizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryCubePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryReportPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-06-20 12:30:57.000000 aliyun-python-sdk-quickbi-public-2.1.3/setup.py
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/LICENSE` & `aliyun-python-sdk-quickbi-public-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/PKG-INFO` & `aliyun-python-sdk-quickbi-public-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-quickbi-public
-Version: 2.1.2
+Version: 2.1.3
 Summary: The quickbi-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-quickbi-public
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/README.rst` & `aliyun-python-sdk-quickbi-public-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-quickbi-public
-Version: 2.1.2
+Version: 2.1.3
 Summary: The quickbi-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-quickbi-public
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,23 +48,27 @@
 aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
 aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py
+aliyunsdkquickbi_public/request/v20220101/QueryComponentPerformanceRequest.py
+aliyunsdkquickbi_public/request/v20220101/QueryCubeOptimizationRequest.py
+aliyunsdkquickbi_public/request/v20220101/QueryCubePerformanceRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py
+aliyunsdkquickbi_public/request/v20220101/QueryReportPerformanceRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py
 aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.3/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.2/setup.py` & `aliyun-python-sdk-quickbi-public-2.1.3/setup.py`

 * *Files identical despite different names*

