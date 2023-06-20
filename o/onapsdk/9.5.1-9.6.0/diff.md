# Comparing `tmp/onapsdk-9.5.1.tar.gz` & `tmp/onapsdk-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onapsdk-9.5.1.tar", last modified: Mon Jun 27 08:40:05 2022, max compression
+gzip compressed data, was "onapsdk-9.6.0.tar", last modified: Fri Jul  8 15:00:10 2022, max compression
```

## Comparing `onapsdk-9.5.1.tar` & `onapsdk-9.6.0.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.226498 onapsdk-9.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-27 08:39:52.000000 onapsdk-9.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5531 2022-06-27 08:40:05.226498 onapsdk-9.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2022-06-27 08:39:52.000000 onapsdk-9.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1214 2022-06-27 08:40:05.227498 onapsdk-9.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-27 08:39:52.000000 onapsdk-9.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.163493 onapsdk-9.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.172494 onapsdk-9.5.1/src/onapsdk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.175495 onapsdk-9.5.1/src/onapsdk/aai/
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5732 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/aai_element.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/bulk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.180495 onapsdk-9.5.1/src/onapsdk/aai/business/
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22941 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/customer.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     3416 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/line_of_business.py
--rw-rw-rw-   0 root         (0) root         (0)    10792 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/network.py
--rw-rw-rw-   0 root         (0) root         (0)     4408 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/owning_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     3031 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/platform.py
--rw-rw-rw-   0 root         (0) root         (0)    11929 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/pnf.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/project.py
--rw-rw-rw-   0 root         (0) root         (0)    21487 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/service.py
--rw-rw-rw-   0 root         (0) root         (0)     6384 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/sp_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     8364 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/vf_module.py
--rw-rw-rw-   0 root         (0) root         (0)    25255 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/business/vnf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.181495 onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)      168 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25067 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/cloud_region.py
--rw-rw-rw-   0 root         (0) root         (0)    11526 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/complex.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/tenant.py
--rw-rw-rw-   0 root         (0) root         (0)     5333 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/service_design_and_creation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.187495 onapsdk-9.5.1/src/onapsdk/aai/templates/
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_add_relationship.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      249 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_bulk.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_line_of_business_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_owning_entity_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_platform_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       44 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_project_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_service_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2361 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_service_instance_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      601 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/aai_sp_partner_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_add_availability_zone.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1537 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_add_esr_system_info.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_add_tenant.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      987 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/complex_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/customer_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       40 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/aai/templates/customer_service_subscription_create.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.189495 onapsdk-9.5.1/src/onapsdk/cds/
--rw-rw-rw-   0 root         (0) root         (0)      191 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18808 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/blueprint.py
--rw-rw-rw-   0 root         (0) root         (0)     8384 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/blueprint_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/blueprint_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/cds_element.py
--rw-rw-rw-   0 root         (0) root         (0)     8060 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/data_dictionary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.190496 onapsdk-9.5.1/src/onapsdk/cds/templates/
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/templates/cds_blueprintprocessor_bootstrap.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2021 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/templates/data_dictionary_base.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      311 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cds/templates/data_dictionary_source_rest.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.191496 onapsdk-9.5.1/src/onapsdk/clamp/
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/clamp_element.py
--rw-rw-rw-   0 root         (0) root         (0)    12861 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/loop_instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.192496 onapsdk-9.5.1/src/onapsdk/clamp/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_MinMax_config.json.j2
--rw-rw-rw-   0 root         (0) root         (0)    12980 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_drools_policy.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2788 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_frequency.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      883 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_tca_config.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.193496 onapsdk-9.5.1/src/onapsdk/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/configuration/global_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/configuration/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.195496 onapsdk-9.5.1/src/onapsdk/cps/
--rw-rw-rw-   0 root         (0) root         (0)      285 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5000 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cps/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cps/cps_element.py
--rw-rw-rw-   0 root         (0) root         (0)     5357 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cps/dataspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/cps/schemaset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.196496 onapsdk-9.5.1/src/onapsdk/dmaap/
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/dmaap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/dmaap/dmaap.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/dmaap/dmaap_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.197496 onapsdk-9.5.1/src/onapsdk/msb/
--rw-rw-rw-   0 root         (0) root         (0)      201 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3411 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/esr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.199496 onapsdk-9.5.1/src/onapsdk/msb/k8s/
--rw-rw-rw-   0 root         (0) root         (0)      211 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/k8s/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2971 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/k8s/connectivity_info.py
--rw-rw-rw-   0 root         (0) root         (0)    12837 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/k8s/definition.py
--rw-rw-rw-   0 root         (0) root         (0)     5542 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/k8s/instance.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/msb_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/multicloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.201496 onapsdk-9.5.1/src/onapsdk/msb/templates/
--rw-rw-rw-   0 root         (0) root         (0)      997 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/msb_esr_vim_registration.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_add_connectivity_info.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_add_definition.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_create_configuration_template.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_create_profile_for_definition.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_instantiate.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.201496 onapsdk-9.5.1/src/onapsdk/nbi/
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/nbi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17453 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/nbi/nbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.202496 onapsdk-9.5.1/src/onapsdk/nbi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      755 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/nbi/templates/nbi_service_order_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)    11649 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/onap_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.206497 onapsdk-9.5.1/src/onapsdk/sdc/
--rw-rw-rw-   0 root         (0) root         (0)    14837 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7735 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/category_management.py
--rw-rw-rw-   0 root         (0) root         (0)     5446 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/component.py
--rw-rw-rw-   0 root         (0) root         (0)     2481 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/pnf.py
--rw-rw-rw-   0 root         (0) root         (0)     5645 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/sdc_element.py
--rw-rw-rw-   0 root         (0) root         (0)    33975 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/sdc_resource.py
--rw-rw-rw-   0 root         (0) root         (0)    35163 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.212497 onapsdk-9.5.1/src/onapsdk/sdc/templates/
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/add_artifact_to_vf.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/add_resource_to_service.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      984 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/component_declare_input.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      781 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/pnf_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_element_action.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       44 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_action.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_deployment_artifact.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1371 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_input.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1174 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_nested_input.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      422 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_property.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      697 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_category.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      404 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_component_set_property_value.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_set_input_default_value.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      404 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_set_property_value.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      788 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/service_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)       81 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/vendor_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      750 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/vf_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     3365 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/vf_vsp_update.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/templates/vsp_create.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2911 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/vendor.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/vf.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/vfc.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/vl.py
--rw-rw-rw-   0 root         (0) root         (0)    13128 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdc/vsp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.213497 onapsdk-9.5.1/src/onapsdk/sdnc/
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdnc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4990 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdnc/preload.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdnc/sdnc_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.214497 onapsdk-9.5.1/src/onapsdk/sdnc/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1709 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdnc/templates/instantiate_network_ala_carte_upload_preload_gr_api.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1204 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/sdnc/templates/instantiate_vf_module_ala_carte_upload_preload_gr_api.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.215497 onapsdk-9.5.1/src/onapsdk/so/
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7242 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/deletion.py
--rw-rw-rw-   0 root         (0) root         (0)    40219 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/instantiation.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/so_db_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     6796 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/so_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.221498 onapsdk-9.5.1/src/onapsdk/so/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1270 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/add_cloud_site_with_identity_service.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      757 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/deletion_network.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1036 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/deletion_service.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1194 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/deletion_vf_module.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1175 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/deletion_vnf.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     5102 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_multi_vnf_service_macro.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_network_ala_carte.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1465 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_network_vnf_ala_carte_base.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_service_ala_carte.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     9375 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_service_macro.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2694 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vf_module_ala_carte.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      632 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_ala_carte.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     8059 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_macro.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     7757 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_macro_so_vnf.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      216 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/service_instance_model_info.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      624 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/vf_model_info.json.j2
--rw-rw-rw-   0 root         (0) root         (0)      349 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/so/templates/vnf_model_info.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.223498 onapsdk-9.5.1/src/onapsdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)      718 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/headers_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/jinja.py
--rw-rw-rw-   0 root         (0) root         (0)     2671 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     2858 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/utils/tosca_file_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.224498 onapsdk-9.5.1/src/onapsdk/ves/
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.225498 onapsdk-9.5.1/src/onapsdk/ves/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3547 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/templates/ves7_batch_with_stndDefined_valid.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1669 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/templates/ves_stnd_event.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     1543 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/templates/ves_stnd_valid_event.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     2472 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/ves.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/ves/ves_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.226498 onapsdk-9.5.1/src/onapsdk/vid/
--rw-rw-rw-   0 root         (0) root         (0)      128 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/vid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.226498 onapsdk-9.5.1/src/onapsdk/vid/templates/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/vid/templates/vid_declare_resource.json.j2
--rw-rw-rw-   0 root         (0) root         (0)     3347 2022-06-27 08:39:52.000000 onapsdk-9.5.1/src/onapsdk/vid/vid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 08:40:05.174494 onapsdk-9.5.1/src/onapsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5531 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7355 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      118 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-06-27 08:40:05.000000 onapsdk-9.5.1/src/onapsdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.912890 onapsdk-9.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-07-08 14:59:58.000000 onapsdk-9.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5531 2022-07-08 15:00:10.912890 onapsdk-9.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2022-07-08 14:59:58.000000 onapsdk-9.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2022-07-08 15:00:10.913890 onapsdk-9.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-07-08 14:59:58.000000 onapsdk-9.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.847921 onapsdk-9.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.857916 onapsdk-9.6.0/src/onapsdk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.861914 onapsdk-9.6.0/src/onapsdk/aai/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5732 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/aai_element.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/bulk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.865913 onapsdk-9.6.0/src/onapsdk/aai/business/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22941 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     3416 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/line_of_business.py
+-rw-rw-rw-   0 root         (0) root         (0)    10792 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/network.py
+-rw-rw-rw-   0 root         (0) root         (0)     4408 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/owning_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)    12338 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/pnf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    21487 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6384 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/sp_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8364 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/vf_module.py
+-rw-rw-rw-   0 root         (0) root         (0)    25255 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/business/vnf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.867912 onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25067 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/cloud_region.py
+-rw-rw-rw-   0 root         (0) root         (0)    11526 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/complex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/tenant.py
+-rw-rw-rw-   0 root         (0) root         (0)     5333 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/service_design_and_creation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.872909 onapsdk-9.6.0/src/onapsdk/aai/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_add_relationship.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      249 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_bulk.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       62 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_line_of_business_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      106 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_owning_entity_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_platform_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       44 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_project_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_service_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_service_instance_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      601 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/aai_sp_partner_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      273 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_add_availability_zone.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_add_esr_system_info.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_add_tenant.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      987 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/complex_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      480 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/customer_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       40 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/aai/templates/customer_service_subscription_create.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.874908 onapsdk-9.6.0/src/onapsdk/cds/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27227 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/blueprint.py
+-rw-rw-rw-   0 root         (0) root         (0)     8384 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/blueprint_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/blueprint_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/cds_element.py
+-rw-rw-rw-   0 root         (0) root         (0)     8060 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/data_dictionary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.875908 onapsdk-9.6.0/src/onapsdk/cds/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/templates/cds_blueprintprocessor_bootstrap.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/templates/data_dictionary_base.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      311 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cds/templates/data_dictionary_source_rest.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.876907 onapsdk-9.6.0/src/onapsdk/clamp/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/clamp_element.py
+-rw-rw-rw-   0 root         (0) root         (0)    12861 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/loop_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.877907 onapsdk-9.6.0/src/onapsdk/clamp/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_MinMax_config.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)    12980 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_drools_policy.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_frequency.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      883 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_tca_config.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.878906 onapsdk-9.6.0/src/onapsdk/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/configuration/global_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/configuration/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.880905 onapsdk-9.6.0/src/onapsdk/cps/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5000 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cps/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cps/cps_element.py
+-rw-rw-rw-   0 root         (0) root         (0)     5357 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cps/dataspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/cps/schemaset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.881905 onapsdk-9.6.0/src/onapsdk/dmaap/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/dmaap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/dmaap/dmaap.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/dmaap/dmaap_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.882904 onapsdk-9.6.0/src/onapsdk/msb/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/esr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.884904 onapsdk-9.6.0/src/onapsdk/msb/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/k8s/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2971 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/k8s/connectivity_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    12837 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/k8s/definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/k8s/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/msb_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/multicloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.886903 onapsdk-9.6.0/src/onapsdk/msb/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      997 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/msb_esr_vim_registration.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      177 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_add_connectivity_info.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_add_definition.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       86 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_create_configuration_template.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_create_profile_for_definition.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_instantiate.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.886903 onapsdk-9.6.0/src/onapsdk/nbi/
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/nbi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17453 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/nbi/nbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.887902 onapsdk-9.6.0/src/onapsdk/nbi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      755 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/nbi/templates/nbi_service_order_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)    11665 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/onap_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.891900 onapsdk-9.6.0/src/onapsdk/sdc/
+-rw-rw-rw-   0 root         (0) root         (0)    14837 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7735 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/category_management.py
+-rw-rw-rw-   0 root         (0) root         (0)     5446 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/pnf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/sdc_element.py
+-rw-rw-rw-   0 root         (0) root         (0)    33975 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/sdc_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)    35163 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.898897 onapsdk-9.6.0/src/onapsdk/sdc/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/add_artifact_to_vf.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/add_resource_to_service.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      984 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/component_declare_input.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      781 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/pnf_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      111 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_element_action.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       44 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_action.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_deployment_artifact.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_input.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_nested_input.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      422 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_property.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      697 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_category.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      404 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_component_set_property_value.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      180 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_set_input_default_value.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      404 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_set_property_value.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/service_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)       81 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/vendor_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      750 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/vf_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/vf_vsp_update.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/templates/vsp_create.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/vendor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/vf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/vfc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/vl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13128 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdc/vsp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.899896 onapsdk-9.6.0/src/onapsdk/sdnc/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdnc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4990 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdnc/preload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdnc/sdnc_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.899896 onapsdk-9.6.0/src/onapsdk/sdnc/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdnc/templates/instantiate_network_ala_carte_upload_preload_gr_api.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/sdnc/templates/instantiate_vf_module_ala_carte_upload_preload_gr_api.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.901895 onapsdk-9.6.0/src/onapsdk/so/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7242 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/deletion.py
+-rw-rw-rw-   0 root         (0) root         (0)    40219 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/instantiation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/so_db_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6796 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/so_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.907893 onapsdk-9.6.0/src/onapsdk/so/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/add_cloud_site_with_identity_service.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      757 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/deletion_network.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/deletion_service.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/deletion_vf_module.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/deletion_vnf.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_multi_vnf_service_macro.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_network_ala_carte.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_network_vnf_ala_carte_base.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_service_ala_carte.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     9375 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_service_macro.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vf_module_ala_carte.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      632 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_ala_carte.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     8059 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_macro.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     7757 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_macro_so_vnf.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      216 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/service_instance_model_info.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      624 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/vf_model_info.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)      349 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/so/templates/vnf_model_info.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.909892 onapsdk-9.6.0/src/onapsdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      718 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/headers_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/jinja.py
+-rw-rw-rw-   0 root         (0) root         (0)     2671 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     2858 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/utils/tosca_file_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.910891 onapsdk-9.6.0/src/onapsdk/ves/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.911891 onapsdk-9.6.0/src/onapsdk/ves/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/templates/ves7_batch_with_stndDefined_valid.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/templates/ves_stnd_event.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/templates/ves_stnd_valid_event.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/ves.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/ves/ves_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.912890 onapsdk-9.6.0/src/onapsdk/vid/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/vid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.912890 onapsdk-9.6.0/src/onapsdk/vid/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/vid/templates/vid_declare_resource.json.j2
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2022-07-08 14:59:58.000000 onapsdk-9.6.0/src/onapsdk/vid/vid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-08 15:00:10.859915 onapsdk-9.6.0/src/onapsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5531 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7355 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      118 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-07-08 15:00:10.000000 onapsdk-9.6.0/src/onapsdk.egg-info/top_level.txt
```

### Comparing `onapsdk-9.5.1/PKG-INFO` & `onapsdk-9.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onapsdk
-Version: 9.5.1
+Version: 9.6.0
 Summary: SDK to use ONAP Programatically
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/onap/python-onapsdk
 Author: Orange OpenSource
 License: Apache 2.0
 Description: # Python ONAP SDK
         
         an SDK to use ONAP programmatically with Python code
```

### Comparing `onapsdk-9.5.1/README.md` & `onapsdk-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/setup.cfg` & `onapsdk-9.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/aai_element.py` & `onapsdk-9.6.0/src/onapsdk/aai/aai_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/bulk.py` & `onapsdk-9.6.0/src/onapsdk/aai/bulk.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/customer.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/customer.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/instance.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/instance.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/line_of_business.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/line_of_business.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/network.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/network.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/owning_entity.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/owning_entity.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/platform.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/platform.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/pnf.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/pnf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Pnf instance module."""
 
-from typing import Optional, TYPE_CHECKING
+from typing import Iterator, Optional, TYPE_CHECKING
 
 from onapsdk.exceptions import ResourceNotFound
 from .instance import Instance
 
 if TYPE_CHECKING:
     from .service import ServiceInstance  # pylint: disable=cyclic-import
 
@@ -144,14 +144,29 @@
 
         Returns:
             str: Url to get all pnfs
 
         """
         return f"{cls.base_url}{cls.api_version}/network/pnfs/"
 
+    @classmethod
+    def get_all(cls) -> Iterator["PnfInstance"]:
+        """Get all PNF instances.
+
+        Yields:
+            PnfInstance: Pnf instance
+
+        """
+        for pnf_data in cls.send_message_json( \
+            "GET", \
+            "Get all pnf instances", \
+            cls.get_all_url() \
+        ).get("pnf", []):
+            yield cls.create_from_api_response(pnf_data, None)
+
     @property
     def url(self) -> str:
         """Network instance url.
 
         Returns:
             str: NetworkInstance url
```

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/project.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/project.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/service.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/service.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/sp_partner.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/sp_partner.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/vf_module.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/vf_module.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/business/vnf.py` & `onapsdk-9.6.0/src/onapsdk/aai/business/vnf.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/cloud_region.py` & `onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/cloud_region.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/complex.py` & `onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/complex.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/cloud_infrastructure/tenant.py` & `onapsdk-9.6.0/src/onapsdk/aai/cloud_infrastructure/tenant.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/service_design_and_creation.py` & `onapsdk-9.6.0/src/onapsdk/aai/service_design_and_creation.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/templates/aai_service_instance_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/aai/templates/aai_service_instance_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/templates/aai_sp_partner_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/aai/templates/aai_sp_partner_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_add_esr_system_info.json.j2` & `onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_add_esr_system_info.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/templates/cloud_region_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/aai/templates/cloud_region_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/aai/templates/complex_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/aai/templates/complex_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/blueprint.py` & `onapsdk-9.6.0/src/onapsdk/cds/blueprint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # SPDX-License-Identifier: Apache-2.0
 """CDS Blueprint module."""
 import json
 import re
 from dataclasses import dataclass, field
 from datetime import datetime
 from io import BytesIO
-from typing import Any, Dict, Generator, Iterator, List
+from typing import Any, Dict, Generator, Iterator, List, Optional
+from urllib.parse import urlencode
 from uuid import uuid4
 from zipfile import ZipFile
 
 import oyaml as yaml
 
 from onapsdk.utils.jinja import jinja_env
 from onapsdk.exceptions import FileError, ParameterError, ValidationError
@@ -349,14 +350,159 @@
             self.url,
             auth=self.auth,
             data=json.dumps(execution_service_input)
         )
         return response["payload"]
 
 
+class ResolvedTemplate(CdsElement):
+    """Resolved template class.
+
+    Store and retrieve rendered template results.
+    """
+
+    def __init__(self, blueprint: "Blueprint",  # pylint: disable=too-many-arguments
+                 artifact_name: Optional[str] = None,
+                 resolution_key: Optional[str] = None,
+                 resource_id: Optional[str] = None,
+                 resource_type: Optional[str] = None,
+                 occurrence: Optional[str] = None,
+                 response_format: str = "application/json") -> None:
+        """Init resolved template class instance.
+
+        Args:
+            blueprint (Blueprint): Blueprint object.
+            artifact_name (Optional[str], optional): Artifact name for which to retrieve
+                a resolved resource. Defaults to None.
+            resolution_key (Optional[str], optional): Resolution Key associated with
+                the resolution. Defaults to None.
+            resource_id (Optional[str], optional): Resource Id associated with
+                the resolution. Defaults to None.
+            resource_type (Optional[str], optional): Resource Type associated
+                with the resolution. Defaults to None.
+            occurrence (Optional[str], optional): Occurrence of the template resolution (1-n).
+                Defaults to None.
+            response_format (str): Expected format of the template being retrieved.
+
+        """
+        super().__init__()
+        self.blueprint: "Blueprint" = blueprint
+        self.artifact_name: Optional[str] = artifact_name
+        self.resolution_key: Optional[str] = resolution_key
+        self.resource_id: Optional[str] = resource_id
+        self.resource_type: Optional[str] = resource_type
+        self.occurrence: Optional[str] = occurrence
+        self.response_format: str = response_format
+
+    @property
+    def url(self) -> str:
+        """Url property.
+
+        Returns:
+            str: Url
+
+        """
+        return f"{self._url}/api/v1/template"
+
+    @property
+    def resolved_template_url(self) -> str:
+        """Url to retrieve resolved template.
+
+        Filter None parameters.
+
+        Returns:
+            str: Retrieve resolved template url
+
+        """
+        params_dict: Dict[str, str] = urlencode(dict(filter(lambda item: item[1] is not None, {
+            "bpName": self.blueprint.metadata.template_name,
+            "bpVersion": self.blueprint.metadata.template_version,
+            "artifactName": self.artifact_name,
+            "resolutionKey": self.resolution_key,
+            "resourceType": self.resource_type,
+            "resourceId": self.resource_id,
+            "occurrence": self.occurrence,
+            "format": self.response_format
+        }.items())))
+        return f"{self.url}?{params_dict}"
+
+    def get_resolved_template(self) -> Dict[str, str]:
+        """Get resolved template.
+
+        Returns:
+            Dict[str, str]: Resolved template
+
+        """
+        return self.send_message_json(
+            "GET",
+            f"Get resolved template {self.artifact_name} for "
+            f"{self.blueprint.metadata.template_name} version "
+            f"{self.blueprint.metadata.template_version}",
+            self.resolved_template_url,
+            auth=self.auth
+        )
+
+    def store_resolved_template(self, resolved_template: str) -> None:
+        """Store resolved template.
+
+        Args:
+            resolved_template (str): Template to store
+
+        Raises:
+            ParameterError: To store template it's needed to pass artifact name and:
+             - resolution key, or
+             - resource type and resource id.
+            If not all needed parameters are given that exception will be raised.
+
+        """
+        if self.artifact_name and self.resolution_key:
+            return self.store_resolved_template_with_resolution_key(resolved_template)
+        if self.artifact_name and self.resource_type and self.resource_id:
+            return self.store_resolved_template_with_resource_type_and_id(resolved_template)
+        raise ParameterError("To store template artifact name with resolution key or both "
+                             "resource type and id is needed")
+
+    def store_resolved_template_with_resolution_key(self, resolved_template: str) -> None:
+        """Store template using resolution key.
+
+        Args:
+            resolved_template (str): Template to store
+
+        """
+        return self.send_message(
+            "POST",
+            f"Store resolved template {self.artifact_name} for "
+            f"{self.blueprint.metadata.template_name} version "
+            f"{self.blueprint.metadata.template_version}",
+            f"{self.url}/{self.blueprint.metadata.template_name}/"
+            f"{self.blueprint.metadata.template_version}/{self.artifact_name}/"
+            f"{self.resolution_key}",
+            auth=self.auth,
+            data=resolved_template
+        )
+
+    def store_resolved_template_with_resource_type_and_id(self, resolved_template: str) -> None:
+        """Store template using resource type and resource ID.
+
+        Args:
+            resolved_template (str): Template to store
+
+        """
+        return self.send_message(
+            "POST",
+            f"Store resolved template {self.artifact_name} for "
+            f"{self.blueprint.metadata.template_name} version "
+            f"{self.blueprint.metadata.template_version}",
+            f"{self.url}/{self.blueprint.metadata.template_name}/"
+            f"{self.blueprint.metadata.template_version}/{self.artifact_name}/"
+            f"{self.resource_type}/{self.resource_id}",
+            auth=self.auth,
+            data=resolved_template
+        )
+
 class Blueprint(CdsElement):
     """CDS blueprint representation."""
 
     TEMPLATES_RE = r"Templates\/.*json$"
     TOSCA_META = "TOSCA-Metadata/TOSCA.meta"
 
     def __init__(self, cba_file_bytes: bytes) -> None:
@@ -612,7 +758,61 @@
             Workflow: Workflow with given name
 
         """
         try:
             return next(filter(lambda workflow: workflow.name == workflow_name, self.workflows))
         except StopIteration:
             raise ParameterError("Workflow with given name does not exist")
+
+    def get_resolved_template(self,  # pylint: disable=too-many-arguments
+                              artifact_name: str,
+                              resolution_key: Optional[str] = None,
+                              resource_type: Optional[str] = None,
+                              resource_id: Optional[str] = None,
+                              occurrence: Optional[str] = None) -> Dict[str, str]:
+        """Get resolved template for Blueprint.
+
+        Args:
+            artifact_name (str): Resolved template's artifact name
+            resolution_key (Optional[str], optional): Resolved template's resolution key.
+                Defaults to None.
+            resource_type (Optional[str], optional): Resolved template's resource type.
+                Defaults to None.
+            resource_id (Optional[str], optional): Resolved template's resource ID.
+                Defaults to None.
+            occurrence: (Optional[str], optional): Resolved template's occurrence value.
+                Defaults to None.
+
+        Returns:
+            Dict[str, str]: Resolved template
+
+        """
+        return ResolvedTemplate(blueprint=self,
+                                artifact_name=artifact_name,
+                                resolution_key=resolution_key,
+                                resource_type=resource_type,
+                                resource_id=resource_id,
+                                occurrence=occurrence).get_resolved_template()
+
+    def store_resolved_template(self,  # pylint: disable=too-many-arguments
+                                artifact_name: str,
+                                data: str,
+                                resolution_key: Optional[str] = None,
+                                resource_type: Optional[str] = None,
+                                resource_id: Optional[str] = None) -> None:
+        """Store resolved template for Blueprint.
+
+        Args:
+            artifact_name (str): Resolved template's artifact name
+            data (str): Resolved template
+            resolution_key (Optional[str], optional): Resolved template's resolution key.
+                Defaults to None.
+            resource_type (Optional[str], optional): Resolved template's resource type.
+                Defaults to None.
+            resource_id (Optional[str], optional): Resolved template's resource ID.
+                Defaults to None.
+        """
+        ResolvedTemplate(blueprint=self,
+                         artifact_name=artifact_name,
+                         resolution_key=resolution_key,
+                         resource_type=resource_type,
+                         resource_id=resource_id).store_resolved_template(data)
```

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/blueprint_model.py` & `onapsdk-9.6.0/src/onapsdk/cds/blueprint_model.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/blueprint_processor.py` & `onapsdk-9.6.0/src/onapsdk/cds/blueprint_processor.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/cds_element.py` & `onapsdk-9.6.0/src/onapsdk/cds/cds_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/data_dictionary.py` & `onapsdk-9.6.0/src/onapsdk/cds/data_dictionary.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cds/templates/data_dictionary_base.json.j2` & `onapsdk-9.6.0/src/onapsdk/cds/templates/data_dictionary_base.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/clamp_element.py` & `onapsdk-9.6.0/src/onapsdk/clamp/clamp_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/loop_instance.py` & `onapsdk-9.6.0/src/onapsdk/clamp/loop_instance.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_MinMax_config.json.j2` & `onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_MinMax_config.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_drools_policy.json.j2` & `onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_drools_policy.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_frequency.json.j2` & `onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_frequency.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/clamp/templates/clamp_add_tca_config.json.j2` & `onapsdk-9.6.0/src/onapsdk/clamp/templates/clamp_add_tca_config.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/configuration/global_settings.py` & `onapsdk-9.6.0/src/onapsdk/configuration/global_settings.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/configuration/loader.py` & `onapsdk-9.6.0/src/onapsdk/configuration/loader.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/constants.py` & `onapsdk-9.6.0/src/onapsdk/constants.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cps/anchor.py` & `onapsdk-9.6.0/src/onapsdk/cps/anchor.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cps/dataspace.py` & `onapsdk-9.6.0/src/onapsdk/cps/dataspace.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/cps/schemaset.py` & `onapsdk-9.6.0/src/onapsdk/cps/schemaset.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/dmaap/dmaap.py` & `onapsdk-9.6.0/src/onapsdk/dmaap/dmaap.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/exceptions.py` & `onapsdk-9.6.0/src/onapsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/esr.py` & `onapsdk-9.6.0/src/onapsdk/msb/esr.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/k8s/connectivity_info.py` & `onapsdk-9.6.0/src/onapsdk/msb/k8s/connectivity_info.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/k8s/definition.py` & `onapsdk-9.6.0/src/onapsdk/msb/k8s/definition.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/k8s/instance.py` & `onapsdk-9.6.0/src/onapsdk/msb/k8s/instance.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/multicloud.py` & `onapsdk-9.6.0/src/onapsdk/msb/multicloud.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/templates/msb_esr_vim_registration.json.j2` & `onapsdk-9.6.0/src/onapsdk/msb/templates/msb_esr_vim_registration.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/msb/templates/multicloud_k8s_instantiate.json.j2` & `onapsdk-9.6.0/src/onapsdk/msb/templates/multicloud_k8s_instantiate.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/nbi/nbi.py` & `onapsdk-9.6.0/src/onapsdk/nbi/nbi.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/nbi/templates/nbi_service_order_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/nbi/templates/nbi_service_order_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/onap_service.py` & `onapsdk-9.6.0/src/onapsdk/onap_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,16 @@
                 "[%s][%s] response code: %s",
                 cls.server, action,
                 response.status_code if response is not None else "n/a")
             cls._logger.debug(
                 "[%s][%s] response: %s",
                 cls.server, action,
                 response.text if (response is not None and
-                                  response.headers.get("Content-Type", "") == \
-                                      "application/json") else "n/a")
+                                  response.headers.get("Content-Type", "") in \
+                                      ["application/json", "text/plain"]) else "n/a")
 
             response.raise_for_status()
             return response
 
         except HTTPError as cause:
             cls._logger.error("[%s][%s] API returned and error: %s",
                               cls.server, action, headers)
```

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/__init__.py` & `onapsdk-9.6.0/src/onapsdk/sdc/__init__.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/category_management.py` & `onapsdk-9.6.0/src/onapsdk/sdc/category_management.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/component.py` & `onapsdk-9.6.0/src/onapsdk/sdc/component.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/pnf.py` & `onapsdk-9.6.0/src/onapsdk/sdc/pnf.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/properties.py` & `onapsdk-9.6.0/src/onapsdk/sdc/properties.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/sdc_element.py` & `onapsdk-9.6.0/src/onapsdk/sdc/sdc_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/sdc_resource.py` & `onapsdk-9.6.0/src/onapsdk/sdc/sdc_resource.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/service.py` & `onapsdk-9.6.0/src/onapsdk/sdc/service.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/component_declare_input.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/component_declare_input.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/pnf_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/pnf_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_input.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_input.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_add_nested_input.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_add_nested_input.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/sdc_resource_category.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/sdc_resource_category.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/service_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/service_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/vf_create.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/vf_create.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/templates/vf_vsp_update.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdc/templates/vf_vsp_update.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/vendor.py` & `onapsdk-9.6.0/src/onapsdk/sdc/vendor.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/vf.py` & `onapsdk-9.6.0/src/onapsdk/sdc/vf.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/vfc.py` & `onapsdk-9.6.0/src/onapsdk/sdc/vfc.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/vl.py` & `onapsdk-9.6.0/src/onapsdk/sdc/vl.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdc/vsp.py` & `onapsdk-9.6.0/src/onapsdk/sdc/vsp.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdnc/preload.py` & `onapsdk-9.6.0/src/onapsdk/sdnc/preload.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdnc/sdnc_element.py` & `onapsdk-9.6.0/src/onapsdk/sdnc/sdnc_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdnc/templates/instantiate_network_ala_carte_upload_preload_gr_api.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdnc/templates/instantiate_network_ala_carte_upload_preload_gr_api.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/sdnc/templates/instantiate_vf_module_ala_carte_upload_preload_gr_api.json.j2` & `onapsdk-9.6.0/src/onapsdk/sdnc/templates/instantiate_vf_module_ala_carte_upload_preload_gr_api.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/deletion.py` & `onapsdk-9.6.0/src/onapsdk/so/deletion.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/instantiation.py` & `onapsdk-9.6.0/src/onapsdk/so/instantiation.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/so_db_adapter.py` & `onapsdk-9.6.0/src/onapsdk/so/so_db_adapter.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/so_element.py` & `onapsdk-9.6.0/src/onapsdk/so/so_element.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/add_cloud_site_with_identity_service.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/add_cloud_site_with_identity_service.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/deletion_network.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/deletion_network.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/deletion_service.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/deletion_service.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/deletion_vf_module.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/deletion_vf_module.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/deletion_vnf.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/deletion_vnf.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_multi_vnf_service_macro.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_multi_vnf_service_macro.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_network_vnf_ala_carte_base.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_network_vnf_ala_carte_base.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_service_ala_carte.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_service_ala_carte.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_service_macro.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_service_macro.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vf_module_ala_carte.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vf_module_ala_carte.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_ala_carte.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_ala_carte.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_macro.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_macro.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/instantiate_vnf_macro_so_vnf.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/instantiate_vnf_macro_so_vnf.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/so/templates/vf_model_info.json.j2` & `onapsdk-9.6.0/src/onapsdk/so/templates/vf_model_info.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/__init__.py` & `onapsdk-9.6.0/src/onapsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/gui.py` & `onapsdk-9.6.0/src/onapsdk/utils/gui.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/headers_creator.py` & `onapsdk-9.6.0/src/onapsdk/utils/headers_creator.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/jinja.py` & `onapsdk-9.6.0/src/onapsdk/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/mixins.py` & `onapsdk-9.6.0/src/onapsdk/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/utils/tosca_file_handler.py` & `onapsdk-9.6.0/src/onapsdk/utils/tosca_file_handler.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/ves/templates/ves7_batch_with_stndDefined_valid.json.j2` & `onapsdk-9.6.0/src/onapsdk/ves/templates/ves7_batch_with_stndDefined_valid.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/ves/templates/ves_stnd_event.json.j2` & `onapsdk-9.6.0/src/onapsdk/ves/templates/ves_stnd_event.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/ves/templates/ves_stnd_valid_event.json.j2` & `onapsdk-9.6.0/src/onapsdk/ves/templates/ves_stnd_valid_event.json.j2`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/ves/ves.py` & `onapsdk-9.6.0/src/onapsdk/ves/ves.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk/vid/vid.py` & `onapsdk-9.6.0/src/onapsdk/vid/vid.py`

 * *Files identical despite different names*

### Comparing `onapsdk-9.5.1/src/onapsdk.egg-info/PKG-INFO` & `onapsdk-9.6.0/src/onapsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onapsdk
-Version: 9.5.1
+Version: 9.6.0
 Summary: SDK to use ONAP Programatically
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/onap/python-onapsdk
 Author: Orange OpenSource
 License: Apache 2.0
 Description: # Python ONAP SDK
         
         an SDK to use ONAP programmatically with Python code
```

### Comparing `onapsdk-9.5.1/src/onapsdk.egg-info/SOURCES.txt` & `onapsdk-9.6.0/src/onapsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

