# Comparing `tmp/bexhoma-0.6.3.tar.gz` & `tmp/bexhoma-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Benchmark-Experiment-Host-Manager/Benchmark-Experiment-Host-Manager/dist/.tmp-yhit6_2m/bexhoma-0.6.3.tar", last modified: Fri Mar  3 16:50:22 2023, max compression
+gzip compressed data, was "/home/runner/work/Benchmark-Experiment-Host-Manager/Benchmark-Experiment-Host-Manager/dist/.tmp-m7bgjnz0/bexhoma-0.6.4.tar", last modified: Tue Jun 20 13:53:10 2023, max compression
```

## Comparing `bexhoma-0.6.3.tar` & `bexhoma-0.6.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:50:22.000000 bexhoma-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-03 16:50:12.000000 bexhoma-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-03 16:50:12.000000 bexhoma-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-03-03 16:50:22.000000 bexhoma-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-03-03 16:50:12.000000 bexhoma-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78116 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)   169506 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)    43676 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)    85437 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16979 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/scripts/experimentsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/scripts/tpcds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-03-03 16:50:12.000000 bexhoma-0.6.3/bexhoma/scripts/tpch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-03 16:50:22.000000 bexhoma-0.6.3/bexhoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 16:50:22.000000 bexhoma-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-03 16:50:12.000000 bexhoma-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:10.000000 bexhoma-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 13:53:00.000000 bexhoma-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:53:00.000000 bexhoma-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-20 13:53:10.000000 bexhoma-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-20 13:53:00.000000 bexhoma-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82706 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188427 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47260 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92797 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16979 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/scripts/experimentsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/scripts/tpcds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-20 13:53:00.000000 bexhoma-0.6.4/bexhoma/scripts/tpch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:53:10.000000 bexhoma-0.6.4/bexhoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:53:10.000000 bexhoma-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-20 13:53:00.000000 bexhoma-0.6.4/setup.py
```

### Comparing `bexhoma-0.6.3/LICENSE` & `bexhoma-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bexhoma-0.6.3/PKG-INFO` & `bexhoma-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bexhoma
-Version: 0.6.3
+Version: 0.6.4
 Summary: This python tools helps managing DBMS benchmarking experiments in a Kubernetes-based HPC cluster environment. It enables users to configure hardware / software setups for easily repeating tests over varying configurations.
 Home-page: https://github.com/Beuth-Erdelt/Benchmark-Experiment-Host-Manager
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `bexhoma-0.6.3/README.md` & `bexhoma-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bexhoma-0.6.3/bexhoma/clusters.py` & `bexhoma-0.6.4/bexhoma/clusters.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         self.connectionmanagement['singleConnection'] = False
         self.querymanagement = {}
         self.workload = {}
         self.contextdata = self.config['credentials']['k8s']['context'][self.context]
         self.host = 'localhost'
         self.port = self.contextdata['port']
         self.monitoring_active = True
+        self.monitor_cluster_active = False
         # k8s:
         self.namespace = self.contextdata['namespace']
         self.appname = self.config['credentials']['k8s']['appname']
         self.yamlfolder = yamlfolder
         # experiment:
         self.set_experiments(self.config['instances'], self.config['volumes'], self.config['dockers'])
         self.set_experiment(instance, volume, docker, script)
@@ -847,19 +848,31 @@
         self.logger.debug('testbed.execute_command_in_pod({})'.format(fullcommand))
         proc = subprocess.Popen(fullcommand, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         stdout, stderr = proc.communicate()
         try:
             #print(stdout.decode('utf-8'), stderr.decode('utf-8'))
             str_stdout = stdout.decode('utf-8')
             str_stderr = stderr.decode('utf-8')
-            return "", str_stdout, str_stderr
+            if 'Error from server: error dialing backend' in str_stdout or 'Error from server: error dialing backend' in str_stderr:
+                print("Connection error found")
+                self.wait(5)
+                return self.execute_command_in_pod(command=command, pod=pod, container=container, params=params)
+            else:
+                return "", str_stdout, str_stderr
         except Exception as e:
             print(e)
             print(stdout, stderr)
-            return "", stdout, stderr
+            str_stdout = stdout.decode('utf-8')
+            str_stderr = stderr.decode('utf-8')
+            if 'Error from server: error dialing backend' in str_stdout or 'Error from server: error dialing backend' in str_stderr:
+                print("Connection error found")
+                self.wait(5)
+                return self.execute_command_in_pod(command=command, pod=pod, container=container, params=params)
+            else:
+                return "", stdout, stderr
         return "", "", ""
     def check_DBMS_connection(self, ip, port):
         """
         Check if DBMS is open for connections.
         Tries to open a socket to ip:port.
         Returns True if this is possible.
 
@@ -1072,32 +1085,39 @@
             if len(jobname) == 0:
                 jobs = self.get_jobs(app=app, component=component, experiment=experiment, configuration=configuration, client=client)
                 if len(jobs) == 0:
                     return "no job"
                 jobname = jobs[0]
             api_response = self.v1batches.read_namespaced_job_status(jobname, self.namespace)#, label_selector='app='+cluster.appname)
             #pprint(api_response)
+            print("api_response.spec.completions", api_response.spec.completions)
+            print("api_response.status.succeeded", api_response.status.succeeded)
             # returns number of completed pods (!)
             #return api_response.status.succeeded
             # we want status of job (!)
             #self.logger.debug("api_response.status.succeeded = {}".format(api_response.status.succeeded))
             #self.logger.debug("api_response.status.conditions = {}".format(api_response.status.conditions))
+            if api_response.status.succeeded is not None and api_response.spec.completions <= api_response.status.succeeded:
+                print("Number of completions reached")
+                return True
             if api_response.status.succeeded is not None and api_response.status.succeeded > 0 and api_response.status.conditions is not None and len(api_response.status.conditions) > 0:
                 self.logger.debug(api_response.status.conditions[0].type)
                 return api_response.status.conditions[0].type == 'Complete'
             else:
                 return 0
         except ApiException as e:
             print("Exception when calling BatchV1Api->read_namespaced_job_status: %s\n" % e)
             print("Create new access token")
             self.cluster_access()
             self.wait(2)
             # try again, if not failed due to "not found"
             if not e.status == 404:
                 return self.get_job_status(jobname=jobname, app=app, component=component, experiment=experiment, configuration=configuration, client=client)
+            else:
+                return 0
     def delete_job(self, jobname='', app='', component='', experiment='', configuration='', client=''):
         """
         Delete a job given by name or matching a set of labels (component/ experiment/ configuration)
 
         :param jobname: Name of the job we want to delete
         :param app: app the job belongs to
         :param component: Component, for example sut or monitoring
@@ -1237,14 +1257,36 @@
             # there already is a dashboard pod
             return
         else:
             deployment = 'deploymenttemplate-bexhoma-dashboard.yml'
             name = self.create_dashboard_name(app, component)
             self.logger.debug('testbed.start_dashboard({})'.format(deployment))
             self.kubectl('create -f '+self.yamlfolder+deployment)
+    def start_monitoring_cluster(self, app='', component='monitoring'):
+        """
+        Starts the monitoring component and its service.
+        Manifest for node exporters is expected in 'deamonsettemplate-monitoring.yml'.
+
+        :param app: app monitoring belongs to
+        :param component: Component name, should be 'monitoring' typically
+        """
+        self.monitor_cluster_active = True
+        endpoints = self.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+        if len(endpoints) > 0:
+            # dashboard exists
+            self.logger.debug('testbed.start_monitoring_cluster()=exists')
+            return
+        else:
+            self.logger.debug('testbed.start_monitoring_cluster()=deploy')
+            deployment = 'daemonsettemplate-monitoring.yml'
+            #name = self.create_dashboard_name(app, component)
+            #self.logger.debug('testbed.start_monitoring_general({})'.format(deployment))
+            self.kubectl('create -f '+self.yamlfolder+deployment)
+            #deployment = 'deploymenttemplate-bexhoma-prometheus.yml'
+            #self.kubectl('create -f '+self.yamlfolder+deployment)
     def start_messagequeue(self, app='', component='messagequeue'):
         """
         Starts the message queue.
         Manifest is expected in 'deploymenttemplate-bexhoma-messagequeue.yml'
 
         :param app: app the messagequeue belongs to
         :param component: Component name, should be 'messagequeue' typically
@@ -1468,14 +1510,40 @@
         if len(pods_messagequeue) > 0:
             pod_messagequeue = pods_messagequeue[0]
         else:
             pod_messagequeue = 'bexhoma-messagequeue-5ff94984ff-mv9zn'
         self.logger.debug("I am using messagequeue {}".format(pod_messagequeue))
         redisCommand = 'redis-cli set {redisQueue} {value} '.format(redisQueue=queue, value=value)
         self.execute_command_in_pod(command=redisCommand, pod=pod_messagequeue)
+    def get_service_endpoints(self, service_name="bexhoma-service-monitoring-default"):
+        """
+        Returns a list of all endpoints of a service as a list.
+        This is in particular interesting for headless services.
+        It is used to find all nodes in a cluster, if monitoring of cluster is active.
+
+        :param service_name: Name of the service
+        :return: List of IPs of endpoints
+        """
+        #kubectl get endpoints -o jsonpath="{range .items[*]}{.metadata.name},{.subsets[*].addresses[*].ip}{'\n'}{end}"
+        #service_name = "bexhoma-service-monitoring-default"
+        self.logger.debug("get_service_endpoints({})".format(service_name))
+        endpoints = self.kubectl("get endpoints -o jsonpath=\"{range .items[*]}{.metadata.name},{.subsets[*].addresses[*].ip}{'\\n'}{end}\"")
+        try:
+            endpoints_of_service = endpoints.split("\n")
+            for service in endpoints_of_service:
+                if service.startswith(service_name):
+                    #print(service)
+                    endpoints_string = service[service.find(",")+1:]
+                    #print(endpoints_string)
+                    endpoints_list = endpoints_string.split(" ")
+                    self.logger.debug("endpoints: {}".format(endpoints_list))
+                    return endpoints_list
+        except Exception as e:
+            print("Exception when calling get_service_endpoints: %s\n" % e)
+        return []
 
 
 
 # kubectl delete pvc,pods,services,deployments,jobs -l app=bexhoma-client
 
 
 
@@ -1551,24 +1619,38 @@
         :param experiment: Experiment object
         """
         self.experiments.append(experiment)
     def store_pod_log(self, pod_name, container=''):
         """
         Store the log of a pod in a local file in the experiment result folder.
         Optionally the name of a container can be given (mandatory, if pod has multiple containers).
+        If file containing pod log is already present, we do nothing (no update).
 
         :param pod_name: Name of the pod
         :param container: Name of the container
         """
         # write pod log
-        stdout = self.pod_log(pod_name, container)
-        filename_log = self.config['benchmarker']['resultfolder'].replace("\\", "/").replace("C:", "")+"/"+str(self.code)+'/'+pod_name+'.log'
-        f = open(filename_log, "w")
-        f.write(stdout)
-        f.close()
+        if len(container) > 0:
+            filename_log = "{path}/{code}/{pod}.{container}.log".format(path=self.config['benchmarker']['resultfolder'].replace("\\", "/").replace("C:", ""), code=self.code, pod=pod_name, container=container)
+        else:
+            filename_log = "{path}/{code}/{pod}.log".format(path=self.config['benchmarker']['resultfolder'].replace("\\", "/").replace("C:", ""), code=self.code, pod=pod_name)
+        # do not overwrite
+        if not os.path.isfile(filename_log):
+            # max 10 tries to receive the log (timeout might occure)
+            tries = 1
+            while tries<10:
+                stdout = self.pod_log(pod_name, container)
+                if len(stdout) > 0:
+                    f = open(filename_log, "w")
+                    f.write(stdout)
+                    f.close()
+                    return
+                else:
+                    tries = tries + 1
+
 
 
 
 
 
 
 class aws(kubernetes):
@@ -1602,15 +1684,15 @@
         :param clusterconfig: Filename of the configuration of this cluster
         :param experiments_configfolder: Folder where to find experiment files
         :param context: Name of the context to use - important for kubectl to choose the cluster
         :param code: Unique identifier of the experiments
         """
         self.code = code
         kubernetes.__init__(self, clusterconfig=clusterconfig, experiments_configfolder=experiments_configfolder, context=context, yamlfolder=yamlfolder, code=self.code, instance=instance, volume=volume, docker=docker, script=script, queryfile=queryfile)
-        self.cluster = self.contextdata['cluster']
+        self.cluster = self.context#data['cluster']
     def eksctl(self, command):
         """
         Runs an eksctl command.
 
         :param command: An eksctl command
         :return: stdout of the eksctl command
         """
```

### Comparing `bexhoma-0.6.3/bexhoma/configurations.py` & `bexhoma-0.6.4/bexhoma/configurations.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         self.set_connectionmanagement(**self.experiment.connectionmanagement)
         self.set_storage(**self.experiment.storage)
         self.set_nodes(**self.experiment.nodes)
         self.set_maintaining_parameters(**self.experiment.maintaining_parameters)
         self.set_loading_parameters(**self.experiment.loading_parameters)
         self.patch_loading(self.experiment.loading_patch)
         self.set_benchmarking_parameters(**self.experiment.benchmarking_parameters)
+        self.benchmarking_parameters_list = []
         self.additional_labels = dict()
         self.set_additional_labels(**self.experiment.additional_labels)
         self.experiment.add_configuration(self)
         self.dialect = dialect
         self.use_distributed_datasource = False #: True, iff the SUT should mount 'benchmark-data-volume' as source of (non-generated) data
         # scaling of other components
         self.num_worker = worker
@@ -327,14 +328,23 @@
         """
         Sets ENV for benchmarking components.
         Can be set by experiment before creation of configuration.
 
         :param kwargs: Dict of meta data, example 'PARALLEL' => '64'
         """
         self.benchmarking_parameters = kwargs
+    def add_benchmarking_parameters(self, **kwargs):
+        """
+        Sets ENV for benchmarking components.
+        Can be set by experiment before creation of configuration.
+        This generates a list, where each entry corresponds to a set of clients in a sequence of benchmarkers.
+
+        :param kwargs: Dict of meta data, example 'PARALLEL' => '64'
+        """
+        self.benchmarking_parameters_list.append(kwargs)
     def set_loading(self, parallel, num_pods=None):
         """
         Sets job parameters for loading components: Number of parallel pods and optionally (if different) total number of pods.
         By default total number of pods is set to number of parallel pods.
         Can be set by experiment before creation of configuration.
 
         :param parallel: Number of parallel pods
@@ -539,14 +549,15 @@
         """
         if len(app) == 0:
             app = self.appname
         if len(configuration) == 0:
             configuration = self.configuration
         if len(experiment) == 0:
             experiment = self.code
+        self.logger.debug("start_loading_pod({})".format(configuration))
         # put list of clients to message queue
         redisQueue = '{}-{}-{}-{}'.format(app, component, self.configuration, self.code)
         for i in range(1, self.num_loading+1):
             #redisClient.rpush(redisQueue, i)
             self.experiment.cluster.add_to_messagequeue(queue=redisQueue, data=i)
         # reset number of clients
         redisQueue = '{}-{}-{}-{}'.format(app, 'loader-podcount', self.configuration, self.code)
@@ -560,14 +571,15 @@
         Starts data ingestion by calling scripts inside the sut (dbms) container.
 
         :param delay: Number of seconds to wait after calling scripts
         """
         app = self.appname
         component = 'sut'
         configuration = self.configuration
+        self.logger.debug("start_loading({})".format(configuration))
         pods = self.experiment.cluster.get_pods(app, component, self.experiment.code, configuration)
         if len(pods) > 0:
             pod_sut = pods[0]
             status = self.experiment.cluster.get_pod_status(pod_sut)
             if status != "Running":
                 return False
             if self.num_worker > 0:
@@ -737,26 +749,43 @@
     static_configs:
       - targets: ['{master}:9300']
   - job_name: 'monitor-gpu'
     scrape_interval: {prometheus_interval}
     scrape_timeout: {prometheus_timeout}
     static_configs:
       - targets: ['{master}:9400']""".format(master=name_sut, prometheus_interval=self.prometheus_interval, prometheus_timeout=self.prometheus_timeout)
+                        # service of cluster
+                        endpoints_cluster = self.experiment.cluster.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+                        i = 0
+                        for endpoint in endpoints_cluster:
+                            #print('Worker: {worker}.{service_sut}'.format(worker=pod, service_sut=name_worker))
+                            prometheus_config += """
+  - job_name: '{endpoint}'
+    scrape_interval: {prometheus_interval}
+    scrape_timeout: {prometheus_timeout}
+    static_configs:
+      - targets: ['{endpoint}:9300']""".format(endpoint=endpoint, client=i, prometheus_interval=self.prometheus_interval, prometheus_timeout=self.prometheus_timeout)
+                            i = i + 1
                         # services of workers
-                        name_worker = self.generate_component_name(component='worker', configuration=self.configuration, experiment=self.code)
-                        pods_worker = self.experiment.cluster.get_pods(component='worker', configuration=self.configuration, experiment=self.code)
+                        endpoints_worker = self.get_worker_endpoints()
+                        #name_worker = self.generate_component_name(component='worker', configuration=self.configuration, experiment=self.code)
+                        #pods_worker = self.experiment.cluster.get_pods(component='worker', configuration=self.configuration, experiment=self.code)
                         i = 0
-                        for pod in pods_worker:
-                            print('Worker: {worker}.{service_sut}'.format(worker=pod, service_sut=name_worker))
+                        #for pod in pods_worker:
+                        for endpoint in endpoints_worker:
+                            if endpoint in endpoints_cluster:
+                                # we already monitor this endpoint
+                                continue
+                            #print('Worker: {worker}.{service_sut}'.format(worker=pod, service_sut=name_worker))
                             prometheus_config += """
-  - job_name: '{worker}'
+  - job_name: '{endpoint}'
     scrape_interval: {prometheus_interval}
     scrape_timeout: {prometheus_timeout}
     static_configs:
-      - targets: ['{worker}.{service_sut}:9300']""".format(worker=pod, service_sut=name_worker, client=i, prometheus_interval=self.prometheus_interval, prometheus_timeout=self.prometheus_timeout)
+      - targets: ['{endpoint}:9300']""".format(endpoint=endpoint, client=i, prometheus_interval=self.prometheus_interval, prometheus_timeout=self.prometheus_timeout)
                             i = i + 1
                         for i,e in enumerate(envs):
                             if e['name'] == 'BEXHOMA_SERVICE':
                                 dep['spec']['template']['spec']['containers'][0]['env'][i]['value'] = name_sut
                             if e['name'] == 'DBMSBENCHMARKER_CONFIGURATION':
                                 dep['spec']['template']['spec']['containers'][0]['env'][i]['value'] = configuration
                             if e['name'] == 'BEXHOMA_WORKERS':
@@ -1064,14 +1093,16 @@
                     #envs = container['env']
                     #for num_env, e in enumerate(envs):
                     #    env_manifest[e['name']] = e['value']
                     #print(env_manifest)
                     #env_merged = {**env_manifest, **env}
                     #print(env_merged)
                     self.logger.debug('configuration.create_manifest_statefulset({})'.format(env))
+                    if not 'env' in dep['spec']['template']['spec']['containers'][i_container]:
+                        dep['spec']['template']['spec']['containers'][i_container]['env'] = []
                     #dep['spec']['template']['spec']['containers'][i_container]['env'] = []
                     for i_env,e in env.items():
                         dep['spec']['template']['spec']['containers'][i_container]['env'].append({'name':i_env, 'value':str(e)})
                 # remove volumes
                 for j, vol in enumerate(dep['spec']['template']['spec']['volumes']):
                     if vol['name'] == 'bexhoma-workers':
                         #print(vol['mountPath'])
@@ -1185,15 +1216,15 @@
                                     #print(vol['mountPath'])
                                     if not use_data:
                                         del result[key]['spec']['template']['spec']['containers'][i]['volumeMounts'][j]
                         if self.dockerimage:
                             result[key]['spec']['template']['spec']['containers'][i]['image'] = self.dockerimage
                         else:
                             self.dockerimage = result[key]['spec']['template']['spec']['containers'][i]['image']
-                    elif not self.monitoring_active:
+                    elif not self.monitoring_active or self.experiment.cluster.monitor_cluster_active:
                         # remove monitoring containers
                         if container['name'] == 'cadvisor':
                             del result[key]['spec']['template']['spec']['containers'][i]
                         if container['name'] == 'dcgm-exporter':
                             del result[key]['spec']['template']['spec']['containers'][i]
                 if 'volumes' in dep['spec']['template']['spec']:
                     for i, vol in reversed(list(enumerate(dep['spec']['template']['spec']['volumes']))):
@@ -1552,15 +1583,15 @@
         #print(timestamp_local)
         return int(timestamp_remote)-int(timestamp_local)
     def get_host_diskspace_used_data(self):
         """
         Returns information about the sut's host disk space used for the data (the database) in kilobyte.
         Basically this calls `du` on the host directory that is mentioned in cluster.config as to store the database.
 
-        :return: Size of disk used for database in Bytes
+        :return: Size of disk used for database in Kilobytes
         """
         self.logger.debug('configuration.get_host_diskspace_used_data()')
         cmd = {}
         if 'datadir' in self.dockertemplate:
             datadir = self.dockertemplate['datadir']
         else:
             return 0
@@ -1583,15 +1614,15 @@
                 return 0
         return 0
     def get_host_diskspace_used(self):
         """
         Returns information about the sut's host disk space.
         Basically this calls `df /` on the host.
 
-        :return: Size of disk in Bytes
+        :return: Size of disk in Kilobytes
         """
         self.logger.debug('configuration.get_host_diskspace_used()')
         disk = ''
         cmd = {}
         try:
             command = "df / | awk 'NR == 2{print \\$3}'"
             #fullcommand = 'kubectl exec '+self.pod_sut+' --container=dbms -- bash -c "'+command+'"'
@@ -1600,18 +1631,21 @@
             disk = stdout#os.popen(fullcommand).read()
             return int(disk.replace('\n',''))
         except Exception as e:
             # Windows
             command = "df / | awk 'NR == 2{print $3}'"
             #fullcommand = 'kubectl exec '+self.pod_sut+' --container=dbms -- bash -c "'+command+'"'
             #disk = os.popen(fullcommand).read()
-            stdin, stdout, stderr = self.execute_command_in_pod_sut(command=command)
-            disk = stdout#os.popen(fullcommand).read()
-            if len(disk) > 0:
-                return int(disk.replace('\n',''))
+            try:
+                stdin, stdout, stderr = self.execute_command_in_pod_sut(command=command)
+                disk = stdout#os.popen(fullcommand).read()
+                if len(disk) > 0:
+                    return int(disk.replace('\n',''))
+            except Exception as e:
+                return 0
         # pipe to awk sometimes does not work
         #return int(disk.split('\t')[0])
         return 0
     def get_host_all(self):
         """
         Calls all `get_host_x()` methods.
         Returns information about the sut's host as a dict.
@@ -1626,14 +1660,27 @@
         server['Cores'] = self.get_host_cores()
         server['host'] = self.get_host_system()
         server['node'] = self.get_host_node()
         server['disk'] = self.get_host_diskspace_used()
         server['datadisk'] = self.get_host_diskspace_used_data()
         server['cuda'] = self.get_host_cuda()
         return server
+    def set_metric_of_config(self, metric, host, gpuid):
+        """
+        Returns a promql query.
+        Parameters in this query are substituted, so that prometheus finds the correct metric.
+        Example: In 'sum(irate(container_cpu_usage_seconds_total{{container_label_io_kubernetes_pod_name=~"(.*){configuration}-{experiment}(.*)", container_label_io_kubernetes_pod_name=~"(.*){configuration}-{experiment}(.*)", container_label_io_kubernetes_container_name="dbms"}}[1m]))'
+        configuration and experiment are placeholders and will be replaced by concrete values.
+
+        :param metric: Parametrized promql query
+        :param host: Name of the host the metrics should be collected from
+        :param gpuid: GPU that the metrics should watch
+        :return: promql query without parameters
+        """
+        return metric.format(host=host, gpuid=gpuid, configuration=self.configuration.lower(), experiment=self.code)
     def get_connection_config(self, connection, alias='', dialect='', serverip='localhost', monitoring_host='localhost'):
         """
         Returns information about the sut's host disk space.
         Basically this calls `df /` on the host.
 
         :return: Size of disk in Bytes
         """
@@ -1717,15 +1764,16 @@
                 if len(c['hostsystem']['GPUIDs']) > 0:
                     gpuid = '|'.join(c['hostsystem']['GPUIDs'])
                 else:
                     gpuid = ""
                 node = c['hostsystem']['node']
                 for metricname, metricdata in config_K8s['monitor']['metrics'].items():
                     c['monitoring']['metrics'][metricname] = metricdata.copy()
-                    c['monitoring']['metrics'][metricname]['query'] = c['monitoring']['metrics'][metricname]['query'].format(host=node, gpuid=gpuid, configuration=self.configuration.lower(), experiment=self.code)
+                    #c['monitoring']['metrics'][metricname]['query'] = c['monitoring']['metrics'][metricname]['query'].format(host=node, gpuid=gpuid, configuration=self.configuration.lower(), experiment=self.code)
+                    c['monitoring']['metrics'][metricname]['query'] = self.set_metric_of_config(metric=c['monitoring']['metrics'][metricname]['query'], host=node, gpuid=gpuid)
         c['JDBC']['url'] = c['JDBC']['url'].format(serverip=serverip, dbname=self.experiment.volume, DBNAME=self.experiment.volume.upper(), timout_s=c['connectionmanagement']['timeout'], timeout_ms=c['connectionmanagement']['timeout']*1000)
         #print(c)
         return c#.copy()
     def OLD_fetch_metrics_loading(self, connection=None, configuration=''):
         self.logger.debug('configuration.fetch_metrics()')
         # set general parameter
         resultfolder = self.experiment.cluster.config['benchmarker']['resultfolder']
@@ -1733,15 +1781,15 @@
         if connection is None:
             connection = self.configuration
         if len(configuration) == 0:
             configuration = connection
         code = self.code
         # get connection config (sut)
         monitoring_host = self.generate_component_name(component='monitoring', configuration=configuration, experiment=self.code)
-        service_name = self.generate_component_name(component='sut', configuration=configuration, experiment=self.code)
+        service_name = self.get_service_sut(configuration=configuration)#self.generate_component_name(component='sut', configuration=configuration, experiment=self.code)
         service_namespace = self.experiment.cluster.contextdata['namespace']
         service_host = self.experiment.cluster.contextdata['service_sut'].format(service=service_name, namespace=service_namespace)
         pods = self.experiment.cluster.get_pods(component='sut', configuration=configuration, experiment=self.code)
         self.pod_sut = pods[0]
         c = self.get_connection_config(connection, serverip=service_host, monitoring_host=monitoring_host)
         print(c)
         connection_data = c
@@ -1823,15 +1871,15 @@
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         time_now = str(datetime.now())
         time_now_int = int(datetime.timestamp(datetime.strptime(time_now,'%Y-%m-%d %H:%M:%S.%f')))
         self.current_benchmark_start = int(time_now_int)
         # get connection config (sut)
         monitoring_host = self.generate_component_name(component='monitoring', configuration=configuration, experiment=self.code)
-        service_name = self.generate_component_name(component='sut', configuration=configuration, experiment=self.code)
+        service_name = self.get_service_sut(configuration=configuration)#self.generate_component_name(component='sut', configuration=configuration, experiment=self.code)
         service_namespace = self.experiment.cluster.contextdata['namespace']
         service_host = self.experiment.cluster.contextdata['service_sut'].format(service=service_name, namespace=service_namespace)
         pods = self.experiment.cluster.get_pods(component='sut', configuration=configuration, experiment=self.code)
         self.pod_sut = pods[0]
         #service_port = config_K8s['port']
         c = self.get_connection_config(connection, alias, dialect, serverip=service_host, monitoring_host=monitoring_host)#config_K8s['ip'])
         #c['parameter'] = {}
@@ -1861,15 +1909,21 @@
             code=code
             )
         #self.benchmark.code = '1611607321'
         self.code = self.benchmark.code
         #print("Code", self.code)
         self.logger.debug('configuration.run_benchmarker_pod(Code={})'.format(self.code))
         # read config for benchmarker
-        connectionfile = experiments_configfolder+'/connections.config'
+        # empty template:
+        #connectionfile = experiments_configfolder+'/connections.config'
+        # collecting all configs of experiment in result folder
+        connectionfile = self.benchmark.path+'/connections.config'
+        if not os.path.isfile(connectionfile):
+            # empty template:
+            connectionfile = experiments_configfolder+'/connections.config'
         if self.experiment.queryfile is not None:
             queryfile = experiments_configfolder+'/'+self.experiment.queryfile
         else:
             queryfile = experiments_configfolder+'/queries.config'
         self.benchmark.getConfig(connectionfile=connectionfile, queryfile=queryfile)
         if c['name'] in self.benchmark.dbms:
             print("Rerun connection "+connection)
@@ -1883,14 +1937,15 @@
         self.benchmark.dbms[c['name']] = tools.dbms(c, False)
         # copy or generate config folder (query and connection)
         # add connection to existing list
         # or: generate new connection list
         filename = self.benchmark.path+'/connections.config'
         with open(filename, 'w') as f:
             f.write(str(self.benchmark.connections))
+        print(str(self.benchmark.connections))
         filename = self.benchmark.path+'/'+c['name']+'.config'
         with open(filename, 'w') as f:
             f.write(str([c]))
         # write appended query config
         if len(self.experiment.workload) > 0:
             for k,v in self.experiment.workload.items():
                 self.benchmark.queryconfig[k] = v
@@ -1990,23 +2045,65 @@
             stdout = self.experiment.cluster.kubectl('cp --container dashboard '+self.path+'/protocol.json '+pod_dashboard+':/results/'+str(self.code)+'/protocol.json')
             self.logger.debug('copy config protocol.json: {}'.format(stdout))
             """
             # get monitoring for loading
             if self.monitoring_active:
                 cmd = {}
                 #cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(connection, c['name']+'.config', '/results/'+self.code, self.code, self.timeLoadingStart, self.timeLoadingEnd)
-                cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -db -ct loading -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(connection, c['name']+'.config', '/results/'+self.code, self.code, self.timeLoadingStart, self.timeLoadingEnd)
+                cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -db -ct loading -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(
+                    connection, 
+                    c['name']+'.config', 
+                    '/results/'+self.code, 
+                    self.code, 
+                    self.timeLoadingStart, 
+                    self.timeLoadingEnd)
                 stdin, stdout, stderr = self.experiment.cluster.execute_command_in_pod(command=cmd['fetch_loading_metrics'], pod=pod_dashboard, container="dashboard")
                 self.logger.debug(stdout)
                 self.logger.debug(stderr)
                 # upload connections infos again, metrics has overwritten it
                 filename = 'connections.config'
                 cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
                 stdout = self.experiment.cluster.kubectl(cmd['upload_connection_file'])
                 self.logger.debug(stdout)
+                # get metrics of loader components
+                # only if general monitoring is on
+                endpoints_cluster = self.experiment.cluster.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+                if len(endpoints_cluster)>0:
+                    # data generator container
+                    cmd['fetch_loader_metrics'] = 'python metrics.py -r /results/ -db -ct datagenerator -cn datagenerator -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(
+                        connection, 
+                        c['name']+'.config', 
+                        '/results/'+self.code, 
+                        self.code, 
+                        self.timeLoadingStart, 
+                        self.timeLoadingEnd)
+                    stdin, stdout, stderr = self.experiment.cluster.execute_command_in_pod(command=cmd['fetch_loader_metrics'], pod=pod_dashboard, container="dashboard")
+                    self.logger.debug(stdout)
+                    self.logger.debug(stderr)
+                    # upload connections infos again, metrics has overwritten it
+                    filename = 'connections.config'
+                    cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
+                    stdout = self.experiment.cluster.kubectl(cmd['upload_connection_file'])
+                    self.logger.debug(stdout)
+                    # data injector container "sensor"
+                    cmd['fetch_loader_metrics'] = 'python metrics.py -r /results/ -db -ct loader -cn sensor -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(
+                        connection, 
+                        c['name']+'.config', 
+                        '/results/'+self.code, 
+                        self.code, 
+                        self.timeLoadingStart, 
+                        self.timeLoadingEnd)
+                    stdin, stdout, stderr = self.experiment.cluster.execute_command_in_pod(command=cmd['fetch_loader_metrics'], pod=pod_dashboard, container="dashboard")
+                    self.logger.debug(stdout)
+                    self.logger.debug(stderr)
+                    # upload connections infos again, metrics has overwritten it
+                    filename = 'connections.config'
+                    cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
+                    stdout = self.experiment.cluster.kubectl(cmd['upload_connection_file'])
+                    self.logger.debug(stdout)
     def execute_command_in_pod_sut(self, command, pod='', container='dbms', params=''):
         """
         Runs an shell command remotely inside a container of a pod.
         This defaults to the current sut's pod and the container "dbms"
 
         :param command: A shell command
         :param pod: The name of the pod - default current sut's pod
@@ -2114,17 +2211,29 @@
             component = 'loading'
             experiment = self.code
             configuration = self.configuration
             success = self.experiment.cluster.get_job_status(app=app, component=component, experiment=experiment, configuration=configuration)
             jobs = self.experiment.cluster.get_jobs(app, component, self.code, configuration)
             # status per job
             for job in jobs:
+                print("Found running job", job)
                 success = self.experiment.cluster.get_job_status(job)
                 self.experiment.cluster.logger.debug('job {} has success status {}'.format(job, success))
                 #print(job, success)
+                # store logs of successful pods
+                pods = self.experiment.cluster.get_job_pods(app=app, component=component, experiment=experiment, configuration=configuration)
+                for pod in pods:
+                    status = self.experiment.cluster.get_pod_status(pod)
+                    print(pod, status)
+                    if status == "Succeeded":
+                        print("Store logs of job {} pod {}".format(job, pod))
+                        container = 'datagenerator'
+                        self.experiment.cluster.store_pod_log(pod_name=pod, container=container)
+                        container = 'sensor'
+                        self.experiment.cluster.store_pod_log(pod_name=pod, container=container)
                 if success:
                     self.experiment.cluster.logger.debug('job {} will be suspended and parallel loading will be considered finished'.format(job, success))
                     # get labels (start) of sut
                     pod_labels = self.experiment.cluster.get_pods_labels(app=app, component='sut', experiment=experiment, configuration=configuration)
                     #print(pod_labels)
                     if len(pod_labels) > 0:
                         pod = next(iter(pod_labels.keys()))
@@ -2137,38 +2246,41 @@
                         if 'timeIndex' in pod_labels[pod]:
                             self.timeIndex = float(pod_labels[pod]['timeIndex'])
                         for key, value in pod_labels[pod].items():
                             if key.startswith("time_"):
                                 time_type = key[len("time_"):]
                                 self.times_scripts[time_type] = float(value)
                     # delete job and all its pods
-                    self.experiment.cluster.delete_job(job)
-                    pods = self.experiment.cluster.get_job_pods(app=app, component=component, experiment=experiment, configuration=configuration)
+                    #pods = self.experiment.cluster.get_job_pods(app=app, component=component, experiment=experiment, configuration=configuration)
                     for pod in pods:
                         status = self.experiment.cluster.get_pod_status(pod)
                         print(pod, status)
+                        print("Store logs of job {} pod {}".format(job, pod))
                         #if status == "Running":
                         # TODO: Find names of containers dynamically
                         container = 'datagenerator'
-                        stdout = self.experiment.cluster.pod_log(pod=pod, container=container)
-                        #stdin, stdout, stderr = self.pod_log(client_pod_name)
-                        filename_log = self.path+'/'+pod+'.'+container+'.log'
-                        f = open(filename_log, "w")
-                        f.write(stdout)
-                        f.close()
+                        self.experiment.cluster.store_pod_log(pod_name=pod, container=container)
+                        #stdout = self.experiment.cluster.pod_log(pod=pod, container=container)
+                        ##stdin, stdout, stderr = self.pod_log(client_pod_name)
+                        #filename_log = self.path+'/'+pod+'.'+container+'.log'
+                        #f = open(filename_log, "w")
+                        #f.write(stdout)
+                        #f.close()
                         #
                         container = 'sensor'
-                        stdout = self.experiment.cluster.pod_log(pod=pod, container='sensor')
-                        #stdin, stdout, stderr = self.pod_log(client_pod_name)
-                        filename_log = self.path+'/'+pod+'.'+container+'.log'
-                        f = open(filename_log, "w")
-                        f.write(stdout)
-                        f.close()
+                        self.experiment.cluster.store_pod_log(pod_name=pod, container=container)
+                        #stdout = self.experiment.cluster.pod_log(pod=pod, container='sensor')
+                        ##stdin, stdout, stderr = self.pod_log(client_pod_name)
+                        #filename_log = self.path+'/'+pod+'.'+container+'.log'
+                        #f = open(filename_log, "w")
+                        #f.write(stdout)
+                        #f.close()
                         self.experiment.cluster.delete_pod(pod)
                     self.experiment.end_loading(job)
+                    self.experiment.cluster.delete_job(job)
                     loading_pods_active = False
                     if self.monitoring_active:
                         #cmd = {}
                         #cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -c {} -ts {} -te {}'.format(self.code, self.timeLoadingStart, self.timeLoadingEnd)
                         #cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -c {} -e {} -ts {} -te {}'.format(connection, self.code, self.timeLoadingStart, self.timeLoadingEnd)
                         #self.experiment.cluster.logger.debug('load_metrics:{}'.format(cmd['fetch_loading_metrics']))
                         #stdout = os.popen(cmd['fetch_loading_metrics']).read()# os.system(fullcommand)
@@ -2251,14 +2363,46 @@
                         else:
                             volume = ''
                         if volume:
                             fullcommand = 'label pvc '+volume+' --overwrite loaded=True timeLoadingEnd="{}" timeLoadingStart="{}" time_ingested={} timeLoading={} time_generated={}'.format(self.timeLoadingEnd, self.timeLoadingStart, loader_time, self.timeLoading, generator_time)
                             #fullcommand = 'label pvc '+volume+' --overwrite loaded=True time_ingested={} timeLoadingStart="{}" timeLoadingEnd="{}" timeLoading={}'.format(loader_time, int(self.timeLoadingStart), int(self.timeLoadingEnd), self.timeLoading)
                             #print(fullcommand)
                             self.experiment.cluster.kubectl(fullcommand)
+                    # get metrics of loader components
+                    #endpoints_cluster = self.experiment.cluster.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+                    # get monitoring for loading
+                    """
+                    if self.monitoring_active and len(endpoints_cluster)>0:
+                        # copy config to pod - dashboard
+                        pods = self.experiment.cluster.get_pods(component='dashboard')
+                        if len(pods) > 0:
+                            pod_dashboard = pods[0]
+                            cmd = {}
+                            connection = self.configuration#self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration)
+                            #cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(connection, c['name']+'.config', '/results/'+self.code, self.code, self.timeLoadingStart, self.timeLoadingEnd)
+                            cmd['fetch_loader_metrics'] = 'python metrics.py -r /results/ -db -ct loader -cn sensor -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(
+                                connection,
+                                'connections.config',
+                                '/results/'+self.code,
+                                self.code,
+                                timing_start,
+                                timing_end)
+                            stdin, stdout, stderr = self.experiment.cluster.execute_command_in_pod(
+                                command=cmd['fetch_loader_metrics'], 
+                                pod=pod_dashboard, 
+                                container="dashboard")
+                            self.logger.debug(stdout)
+                            self.logger.debug(stderr)
+                            # upload connections infos again, metrics has overwritten it
+                            filename = 'connections.config'
+                            cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
+                            stdout = self.experiment.cluster.kubectl(cmd['upload_connection_file'])
+                            self.logger.debug(stdout)
+                    """
+                    # check if there is a post-loading phase
                     if len(self.indexscript):
                         # loading has not finished (there is indexing)
                         self.load_data(scripts=self.indexscript, time_offset=self.timeLoading, time_start_int=self.timeLoadingStart, script_type='indexed')
         else:
             loading_pods_active = False
         # check if asynch loading outside cluster is done
         # only if inside cluster is done
@@ -2295,26 +2439,30 @@
             if 'timeLoading' in pod_labels[pod]:
                 self.timeLoading = float(pod_labels[pod]['timeLoading'])
             for key, value in pod_labels[pod].items():
                 if key.startswith("time_"):
                     time_type = key[len("time_"):]
                     self.times_scripts[time_type] = float(value)
         else:
-            self.loading_started = False
-            self.loading_finished = False
+            # if there are no labels at this pod, loading has not been started or finished
+            # maybe sut has been restarted? then loading may have been stared though
+            # TODO: check if sensible 
+            #self.loading_started = False
+            #self.loading_finished = False
+            pass
     def load_data(self, scripts, time_offset=0, time_start_int=0, script_type='loaded'):
         """
         Start loading data into the sut.
         This runs `load_data_asynch()` as an asynchronous thread.
         At first `prepare_init_dbms()` is run.
         """
         self.logger.debug('configuration.load_data()')
         self.loading_started = True
         self.prepare_init_dbms(scripts)
-        service_name = self.generate_component_name(component='sut', configuration=self.configuration, experiment=self.code)
+        service_name = self.get_service_sut(configuration=self.configuration)#self.generate_component_name(component='sut', configuration=self.configuration, experiment=self.code)
         pods = self.experiment.cluster.get_pods(component='sut', configuration=self.configuration, experiment=self.code)
         self.pod_sut = pods[0]
         scriptfolder = '/tmp/'
         commands = scripts.copy()
         #commands = self.initscript.copy()
         use_storage = self.use_storage()
         if use_storage:
@@ -2350,14 +2498,27 @@
         else:
             with open(file) as f:
                 result = yaml.safe_load_all(f)
                 result = [data for data in result]
                 return result
                 #unpatched = yaml.safe_load(f)
                 #return unpatched
+    def get_service_sut(self, configuration):
+        """
+        Returns the same of the service where to connect to the SUT.
+        This in general is the name of the service of the deployed component.
+        For SUT, that require a component that is not controlled by bexhoma, this may be overwritten.
+
+        :param configuration: name of the configuration
+        :return: name of the configuration's sut's service
+        """
+        app = self.appname
+        experiment = str(int(self.code))
+        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        return servicename
     def create_manifest_job(self, app='', component='benchmarker', experiment='', configuration='', experimentRun='', client='1', parallelism=1, env={}, template='', nodegroup='', num_pods=1, connection='', patch_yaml=''):#, jobname=''):
         """
         Creates a job and sets labels (component/ experiment/ configuration).
 
         :param app: app the job belongs to
         :param component: Component, for example sut or monitoring
         :param experiment: Unique identifier of the experiment
@@ -2374,15 +2535,15 @@
             app = self.appname
         code = str(int(experiment))
         if not experimentRun:
             experimentRun = str(self.num_experiment_to_apply_done+1)
         #connection = configuration
         #if not len(jobname):
         jobname = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=str(client))
-        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        servicename = self.get_service_sut(configuration=configuration)#self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
         #print(jobname)
         # start (create) time of the job
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         time_now = str(datetime.now())
         time_now_int = int(datetime.timestamp(datetime.strptime(time_now,'%Y-%m-%d %H:%M:%S.%f')))
         #self.current_benchmark_start = int(time_now_int)
@@ -2529,15 +2690,15 @@
         self.logger.debug('configuration.create_manifest_benchmarking()')
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=240)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
         e = {'DBMSBENCHMARKER_NOW': now_string,
-            'DBMSBENCHMARKER_START': start_string,
+            'DBMSBENCHMARKER_START': 0,#start_string, # wait until (=0 do not wait)
             'DBMSBENCHMARKER_CLIENT': str(parallelism),
             'DBMSBENCHMARKER_CODE': code,
             'DBMSBENCHMARKER_CONNECTION': connection,
             'BEXHOMA_CONNECTION': connection,
             'DBMSBENCHMARKER_SLEEP': str(60),
             'DBMSBENCHMARKER_ALIAS': alias}
         env = {**env, **e}
@@ -2559,15 +2720,15 @@
         if len(app) == 0:
             app = self.appname
         code = str(int(experiment))
         experimentRun = str(self.num_experiment_to_apply_done+1)
         connection = self.configuration#self.getConnectionName()
         #jobname = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration)
         #self.maintaining_jobname = jobname
-        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        servicename = self.get_service_sut(configuration=configuration)#self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
         #print(jobname)
         self.logger.debug('configuration.create_manifest_maintaining()')
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=180)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
@@ -2612,31 +2773,49 @@
         self.logger.debug('configuration.create_manifest_loading()')
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=60)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
         env = {'DBMSBENCHMARKER_NOW': now_string,
-            'DBMSBENCHMARKER_START': start_string,
+            'DBMSBENCHMARKER_START': 0,#start_string, # wait until (=0 do not wait)
             }
         # store parameters in connection for evaluation
         if len(self.loading_parameters):
             self.connection_parameter['loading_parameters'] = self.loading_parameters
         #print("self.loading_parameters", self.loading_parameters)
         #env = self.loading_parameters
         env = {**env, **self.loading_parameters}
         print("create_manifest_loading:env=", env)
         template = "jobtemplate-loading.yml"
         if len(self.experiment.jobtemplate_loading) > 0:
             template = self.experiment.jobtemplate_loading
         if len(self.jobtemplate_loading) > 0:
             template = self.jobtemplate_loading
         return self.create_manifest_job(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=1, parallelism=parallelism, env=env, template=template, nodegroup='loading', num_pods=num_pods, connection=connection, patch_yaml=self.loading_patch)
-
-
+    def get_worker_pods(self):
+        pods_worker = self.experiment.cluster.get_pods(component='worker', configuration=self.configuration, experiment=self.code)
+        return pods_worker
+    def get_worker_endpoints(self):
+        """
+        Returns all endpoints of a headless service that monitors nodes of a distributed DBMS.
+        These are IPs of cAdvisor instances.
+        The endpoint list is to be filled in a config of an instance of Prometheus.
+        By default, the workers can be found by the name of their component (worker-0 etc).
+
+        :return: list of endpoints
+        """
+        endpoints = []
+        name_worker = self.generate_component_name(component='worker', configuration=self.configuration, experiment=self.code)
+        pods_worker = self.get_worker_pods()
+        for pod in pods_worker:
+            endpoint = '{worker}.{service_sut}'.format(worker=pod, service_sut=name_worker)
+            endpoints.append(endpoint)
+            print('Worker: {endpoint}'.format(endpoint = endpoint))
+        return endpoints
 
 
 
 
 # kubectl delete pvc,pods,services,deployments,jobs -l app=bexhoma-client
 # kubectl delete pvc,pods,services,deployments,jobs -l app=bexhoma -l component=loading
 
@@ -2689,24 +2868,24 @@
         if len(app) == 0:
             app = self.appname
         code = str(int(experiment))
         experimentRun = str(self.num_experiment_to_apply_done+1)
         #connection = configuration
         jobname = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=client)
         #self.benchmarker_jobname = jobname
-        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        servicename = self.get_service_sut(configuration=configuration)#self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
         #print(jobname)
         self.logger.debug('hammerdb.create_manifest_benchmarking({})'.format(jobname))
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=180)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
         env = {'DBMSBENCHMARKER_NOW': now_string,
-            'DBMSBENCHMARKER_START': start_string,
+            'DBMSBENCHMARKER_START': 0,#start_string, # wait until (=0 do not wait)
             'DBMSBENCHMARKER_CLIENT': str(parallelism),
             'DBMSBENCHMARKER_PODS': str(num_pods),
             'DBMSBENCHMARKER_CODE': code,
             'DBMSBENCHMARKER_CONNECTION': connection,
             'BEXHOMA_CONNECTION': connection,
             'DBMSBENCHMARKER_SLEEP': str(60),
             'DBMSBENCHMARKER_ALIAS': alias}
@@ -2767,24 +2946,24 @@
         if len(app) == 0:
             app = self.appname
         code = str(int(experiment))
         experimentRun = str(self.num_experiment_to_apply_done+1)
         #connection = configuration
         jobname = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=client)
         #self.benchmarker_jobname = jobname
-        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        servicename = self.get_service_sut(configuration=configuration)#self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
         #print(jobname)
         self.logger.debug('ycsb.create_manifest_benchmarking({})'.format(jobname))
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=180)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
         env = {'DBMSBENCHMARKER_NOW': now_string,
-            'DBMSBENCHMARKER_START': start_string,
+            'DBMSBENCHMARKER_START': 0,#start_string, # wait until (=0 do not wait)
             'DBMSBENCHMARKER_CLIENT': str(parallelism),
             'DBMSBENCHMARKER_PODS': str(num_pods),
             'DBMSBENCHMARKER_CODE': code,
             'DBMSBENCHMARKER_CONNECTION': connection,
             'BEXHOMA_CONNECTION': connection,
             'DBMSBENCHMARKER_SLEEP': str(60),
             'DBMSBENCHMARKER_ALIAS': alias}
@@ -2844,24 +3023,24 @@
         if len(app) == 0:
             app = self.appname
         code = str(int(experiment))
         experimentRun = str(self.num_experiment_to_apply_done+1)
         #connection = configuration
         jobname = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=client)
         #self.benchmarker_jobname = jobname
-        servicename = self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
+        servicename = self.get_service_sut(configuration=configuration)#self.generate_component_name(app=app, component='sut', experiment=experiment, configuration=configuration)
         #print(jobname)
         self.logger.debug('benchbase.create_manifest_benchmarking({})'.format(jobname))
         # determine start time
         now = datetime.utcnow()
         now_string = now.strftime('%Y-%m-%d %H:%M:%S')
         start = now + timedelta(seconds=180)
         start_string = start.strftime('%Y-%m-%d %H:%M:%S')
         env = {'DBMSBENCHMARKER_NOW': now_string,
-            'DBMSBENCHMARKER_START': start_string,
+            'DBMSBENCHMARKER_START': 0,#start_string, # wait until (=0 do not wait)
             'DBMSBENCHMARKER_CLIENT': str(parallelism),
             'DBMSBENCHMARKER_PODS': str(num_pods),
             'DBMSBENCHMARKER_CODE': code,
             'DBMSBENCHMARKER_CONNECTION': connection,
             'BEXHOMA_CONNECTION': connection,
             'DBMSBENCHMARKER_SLEEP': str(60),
             'DBMSBENCHMARKER_ALIAS': alias}
@@ -2869,17 +3048,149 @@
         env = {**env, **self.benchmarking_parameters}
         #job_experiment = self.experiment.path+'/job-dbmsbenchmarker-{configuration}-{client}.yml'.format(configuration=configuration, client=client)
         return self.create_manifest_job(app=app, component=component, experiment=experiment, configuration=configuration, experimentRun=experimentRun, client=client, parallelism=parallelism, env=env, template="jobtemplate-benchmarking-benchbase.yml", num_pods=num_pods, nodegroup='benchmarking', connection=connection)#, jobname=jobname)
 
 
 
 
+class yugabytedb(default):
+    """
+    :Date: 2022-10-01
+    :Version: 0.6.0
+    :Authors: Patrick K. Erdelt
+
+        Class for managing an DBMS configuation.
+        This is plugged into an experiment object.
+        This class contains specific settings for a YugabyteDB installation.
+        This is handled outside of bexhoma with the official helm chart.
+        The service name is fixed to be "yb-tserver-service"
+
+        :param experiment: Unique identifier of the experiment
+        :param docker: Name of the Docker image
+        :param configuration: Name of the configuration
+        :param script: Unique identifier of the experiment
+        :param alias: Unique identifier of the experiment
+
+        Copyright (C) 2020  Patrick K. Erdelt
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as
+        published by the Free Software Foundation, either version 3 of the
+        License, or (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
+
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    """
+    def get_service_sut(self, configuration):
+        """
+        Returns the same of the service where to connect to the SUT.
+        This in general is the name of the service of the deployed component.
+        For SUT, that require a component that is not controlled by bexhoma, this may be overwritten.
+        Here, always "yb-tserver-service" is returned.
+
+        :param configuration: name of the configuration
+        :return: name of the configuration's sut's service
+        """
+        return "yb-tserver-service"
+
+
+
+
+class kinetica(default):
+    """
+    :Date: 2022-10-01
+    :Version: 0.6.0
+    :Authors: Patrick K. Erdelt
+
+        Class for managing an DBMS configuation.
+        This is plugged into an experiment object.
+        This class contains specific settings for a Kinetica installation.
+        This is handled outside of bexhoma with the official KAgent.
+        The service name is fixed to be "bexhoma-service-kinetica"
+
+        :param experiment: Unique identifier of the experiment
+        :param docker: Name of the Docker image
+        :param configuration: Name of the configuration
+        :param script: Unique identifier of the experiment
+        :param alias: Unique identifier of the experiment
+
+        Copyright (C) 2020  Patrick K. Erdelt
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as
+        published by the Free Software Foundation, either version 3 of the
+        License, or (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
 
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    """
+    def get_service_sut(self, configuration):
+        """
+        Returns the same of the service where to connect to the SUT.
+        This in general is the name of the service of the deployed component.
+        For SUT, that require a component that is not controlled by bexhoma, this may be overwritten.
+        Here, always "bexhoma-service-kinetica" is returned.
 
+        :param configuration: name of the configuration
+        :return: name of the configuration's sut's service
+        """
+        return "bexhoma-service-kinetica"
+    def create_monitoring(self, app='', component='monitoring', experiment='', configuration=''):
+        """
+        Generate a name for the monitoring component.
+        Basically this is `{app}-{component}-{configuration}-{experiment}-{client}`.
+        For Kinetica, the service to be monitored is named 'bexhoma-service-kinetica'.
 
+        :param app: app the component belongs to
+        :param component: Component, for example sut or monitoring
+        :param experiment: Unique identifier of the experiment
+        :param configuration: Name of the dbms configuration
+        """
+        if component == 'sut':
+            name = 'bexhoma-service-kinetica'
+        else:
+            name = self.generate_component_name(app=app, component=component, experiment=experiment, configuration=configuration)
+        self.logger.debug("kinetica.create_monitoring({})".format(name))
+        return name
+    def set_metric_of_config(self, metric, host, gpuid):
+        """
+        Returns a promql query.
+        Parameters in this query are substituted, so that prometheus finds the correct metric.
+        Example: In 'sum(irate(container_cpu_usage_seconds_total{{container_label_io_kubernetes_pod_name=~"(.*){configuration}-{experiment}(.*)", container_label_io_kubernetes_pod_name=~"(.*){configuration}-{experiment}(.*)", container_label_io_kubernetes_container_name="dbms"}}[1m]))'
+        configuration and experiment are placeholders and will be replaced by concrete values.
+        Here: We do not have a SUT that is specific to the experiment or configuration.
+
+        :param metric: Parametrized promql query
+        :param host: Name of the host the metrics should be collected from
+        :param gpuid: GPU that the metrics should watch
+        :return: promql query without parameters
+        """
+        return metric.format(host=host, gpuid=gpuid, configuration='kinetica', experiment='worker')
+    def get_worker_endpoints(self):
+        """
+        Returns all endpoints of a headless service that monitors nodes of a distributed DBMS.
+        These are IPs of cAdvisor instances.
+        The endpoint list is to be filled in a config of an instance of Prometheus.
+        For Kinetica the service is fixed to be 'bexhoma-service-monitoring-default' and does not depend on the experiment.
+
+        :return: list of endpoints
+        """
+        endpoints = self.experiment.cluster.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+        self.logger.debug("kinetica.get_worker_endpoints({})".format(endpoints))
+        return endpoints
```

### Comparing `bexhoma-0.6.3/bexhoma/evaluators.py` & `bexhoma-0.6.4/bexhoma/evaluators.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,24 @@
 import pandas as pd
 import os
 import re
 import matplotlib.pyplot as plt
 pd.set_option("display.max_rows", None)
 pd.set_option('display.max_colwidth', None)
 # Some nice output
-from IPython.display import display, Markdown
+#from IPython.display import display, Markdown
 import pickle
 import json
 import traceback
 
+def natural_sort(l): 
+    convert = lambda text: int(text) if text.isdigit() else text.lower()
+    alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
+    return sorted(l, key=alphanum_key)
+
 class base:
     """
     Basis class for evaluating an experiment.
     Constructor sets
 
       1. `path`: path to result folders
       1. `code`: Id of the experiment (name of result folder)
@@ -267,39 +272,43 @@
 
         :return: DataFrame of loading results
         """
         filename = "bexhoma-loading.all.df.pickle"
         df = pd.read_pickle(self.path+"/"+filename)
         #df#.sort_values(["configuration", "pod"])
         return df
-    def plot(self, df, column, x, y, plot_by=None):
+    def plot(self, df, column, x, y, plot_by=None, kind='line', dict_colors=None, figsize=(12,8)):
         if plot_by is None:
             fig, ax = plt.subplots()
             for key, grp in df.groupby(column):
                 labels = "{} {}".format(key, column)
-                ax = grp.plot(ax=ax, kind='line', x=x, y=y, label=labels)
+                ax = grp.plot(ax=ax, kind=kind, x=x, y=y, title=y, label=labels, figsize=figsize)
                 ax.set_ylim(0,df[y].max())
             plt.legend(loc='best')
-            plt.show()
+            #plt.show()
+            return ax
         else:
             row=0
             col=0
             groups = df.groupby(plot_by)
             #print(len(groups))
             rows = (len(groups)+1)//2
             #print(rows, "rows")
-            fig, axes = plt.subplots(nrows=rows, ncols=2, sharex=True, squeeze=False)
+            fig, axes = plt.subplots(nrows=rows, ncols=2, sharex=True, squeeze=False, figsize=(figsize[0],figsize[1]*rows))
             #print(axes)
             for key1, grp in groups:#df3.groupby(col1):
                 #print(len(axs))
                 for key2, grp2 in grp.groupby(column):
                     #print(grp2)
                     labels = "{} {}, {} {}".format(key1, plot_by, key2, column)
                     #print(row,col)
-                    ax = grp2.plot(ax=axes[row,col], kind='line', x=x, y=y, label=labels, title=y, figsize=(12,8), layout=(rows,2))
+                    if not dict_colors is None and len(dict_colors):
+                        ax = grp2.plot(ax=axes[row,col], kind=kind, x=x, y=y, label=labels, title=y, figsize=figsize, layout=(rows,2), color=dict_colors)
+                    else:
+                        ax = grp2.plot(ax=axes[row,col], kind=kind, x=x, y=y, label=labels, title=y, figsize=figsize, layout=(rows,2))
                     ax.set_ylim(0, df[y].max())
                 col = col + 1
                 if col > 1:
                     row = row + 1
                     col = 0
             plt.legend(loc='best')
             plt.tight_layout()
@@ -407,16 +416,16 @@
             connection_name = re.findall('BEXHOMA_CONNECTION:(.+?)\n', stdout)[0]
             configuration_name = re.findall('BEXHOMA_CONFIGURATION:(.+?)\n', stdout)[0]
             sf = re.findall('SF (.+?)\n', stdout)[0]
             experiment_run = re.findall('BEXHOMA_EXPERIMENT_RUN:(.+?)\n', stdout)[0]
             client = re.findall('BEXHOMA_CLIENT:(.+?)\n', stdout)[0]
             target = re.findall('YCSB_TARGET (.+?)\n', stdout)[0]
             threads = re.findall('YCSB_THREADCOUNT (.+?)\n', stdout)[0]
-            #workload = re.findall('YCSB_WORKLOAD (.+?)\n', stdout)[0]
-            workload = "A"
+            workload = re.findall('YCSB_WORKLOAD (.+?)\n', stdout)[0]
+            #workload = "A"
             pod_count = re.findall('NUM_PODS (.+?)\n', stdout)[0]
             result = []
             #for line in s.split("\n"):
             for line in lines:
                 line = line.strip('\n')
                 cells = line.split(", ")
                 #print(cells)
@@ -459,46 +468,73 @@
             'client':'int',
             'pod':'str',
             'pod_count':'int',
             'threads':'int',
             'target':'int',
             'sf':'int',
             'workload':'str',
+            'operations':'int',
             '[OVERALL].RunTime(ms)':'float',
             '[OVERALL].Throughput(ops/sec)':'float',
-            '[TOTAL_GCS_PS_Scavenge].Count':'int',
-            '[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'float',
-            '[TOTAL_GCS_PS_MarkSweep].Count':'int',
-            '[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'float',
-            '[TOTAL_GCs].Count':'int',
-            '[TOTAL_GC_TIME].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%].Time(%)':'float',
-            '[READ].Operations':'int',
-            '[READ].AverageLatency(us)':'float',
-            '[READ].MinLatency(us)':'float',
-            '[READ].MaxLatency(us)':'float',
-            '[READ].95thPercentileLatency(us)':'float',
-            '[READ].99thPercentileLatency(us)':'float',
-            '[READ].Return=OK':'int',
+            #'[TOTAL_GCS_PS_Scavenge].Count':'int',
+            #'[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'float',
+            #'[TOTAL_GCS_PS_MarkSweep].Count':'int',
+            #'[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'float',
+            #'[TOTAL_GCs].Count':'int',
+            #'[TOTAL_GC_TIME].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%].Time(%)':'float',
             '[CLEANUP].Operations':'int',
             '[CLEANUP].AverageLatency(us)':'float',
             '[CLEANUP].MinLatency(us)':'float',
             '[CLEANUP].MaxLatency(us)':'float',
             '[CLEANUP].95thPercentileLatency(us)':'float',
             '[CLEANUP].99thPercentileLatency(us)':'float',
-            '[UPDATE].Operations':'int',
-            '[UPDATE].AverageLatency(us)':'float',
-            '[UPDATE].MinLatency(us)':'float',
-            '[UPDATE].MaxLatency(us)':'float',
-            '[UPDATE].95thPercentileLatency(us)':'float',
-            '[UPDATE].99thPercentileLatency(us)':'float',
-            '[UPDATE].Return=OK': 'int',
         })
+        if '[READ].Operations'in df_typed.columns:
+            df_typed = df_typed.astype({
+                '[READ].Operations':'int',
+                '[READ].AverageLatency(us)':'float',
+                '[READ].MinLatency(us)':'float',
+                '[READ].MaxLatency(us)':'float',
+                '[READ].95thPercentileLatency(us)':'float',
+                '[READ].99thPercentileLatency(us)':'float',
+                '[READ].Return=OK':'int',
+        })
+        if '[UPDATE].Operations'in df_typed.columns:
+            df_typed = df_typed.astype({
+                '[UPDATE].Operations':'int',
+                '[UPDATE].AverageLatency(us)':'float',
+                '[UPDATE].MinLatency(us)':'float',
+                '[UPDATE].MaxLatency(us)':'float',
+                '[UPDATE].95thPercentileLatency(us)':'float',
+                '[UPDATE].99thPercentileLatency(us)':'float',
+                '[UPDATE].Return=OK': 'int',
+        })
+        if '[INSERT].Operations'in df_typed.columns:
+            df_typed = df_typed.astype({
+                '[INSERT].Operations':'int',
+                '[INSERT].AverageLatency(us)':'float',
+                '[INSERT].MinLatency(us)':'float',
+                '[INSERT].MaxLatency(us)':'float',
+                '[INSERT].95thPercentileLatency(us)':'float',
+                '[INSERT].99thPercentileLatency(us)':'float',
+                '[INSERT].Return=OK': 'int',
+        })
+        if '[SCAN].Operations'in df_typed.columns:
+            df_typed = df_typed.astype({
+                '[SCAN].Operations':'int',
+                '[SCAN].AverageLatency(us)':'float',
+                '[SCAN].MinLatency(us)':'float',
+                '[SCAN].MaxLatency(us)':'float',
+                '[SCAN].95thPercentileLatency(us)':'float',
+                '[SCAN].99thPercentileLatency(us)':'float',
+                '[SCAN].Return=OK':'int',
+            })
         return df_typed
     def benchmarking_aggregate_by_parallel_pods(self, df):
         """
         Transforms a pandas DataFrame collection of benchmarking results to a new DataFrame.
         All result lines belonging to pods being run in parallel will be aggregated.
 
         :param df: DataFrame of results 
@@ -513,46 +549,73 @@
                 'client':'max',
                 'pod':'sum',
                 'pod_count':'count',
                 'threads':'sum',
                 'target':'sum',
                 'sf':'max',
                 'workload':'max',
+                'operations':'sum',
                 '[OVERALL].RunTime(ms)':'max',
                 '[OVERALL].Throughput(ops/sec)':'sum',
-                '[TOTAL_GCS_PS_Scavenge].Count':'sum',
-                '[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'max',
-                '[TOTAL_GCS_PS_MarkSweep].Count':'sum',
-                '[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'max',
-                '[TOTAL_GCs].Count':'sum',
-                '[TOTAL_GC_TIME].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%].Time(%)':'max',
-                '[READ].Operations':'sum',
-                '[READ].AverageLatency(us)':'mean',
-                '[READ].MinLatency(us)':'min',
-                '[READ].MaxLatency(us)':'max',
-                '[READ].95thPercentileLatency(us)':'max',
-                '[READ].99thPercentileLatency(us)':'max',
-                '[READ].Return=OK':'sum',
+                #'[TOTAL_GCS_PS_Scavenge].Count':'sum',
+                #'[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'max',
+                #'[TOTAL_GCS_PS_MarkSweep].Count':'sum',
+                #'[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'max',
+                #'[TOTAL_GCs].Count':'sum',
+                #'[TOTAL_GC_TIME].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%].Time(%)':'max',
                 '[CLEANUP].Operations':'sum',
                 '[CLEANUP].AverageLatency(us)':'mean',
                 '[CLEANUP].MinLatency(us)':'min',
                 '[CLEANUP].MaxLatency(us)':'max',
-                '[CLEANUP].95thPercentileLatency(us)':'max',
-                '[CLEANUP].99thPercentileLatency(us)':'max',
-                '[UPDATE].Operations':'sum',
-                '[UPDATE].AverageLatency(us)':'mean',
-                '[UPDATE].MinLatency(us)':'min',
-                '[UPDATE].MaxLatency(us)':'max',
-                '[UPDATE].95thPercentileLatency(us)':'max',
-                '[UPDATE].99thPercentileLatency(us)':'max',
-                '[UPDATE].Return=OK': 'sum',
+                '[CLEANUP].95thPercentileLatency(us)':'mean',
+                '[CLEANUP].99thPercentileLatency(us)':'mean',
             }
+            if '[READ].Operations' in grp.columns:
+                aggregate = {**aggregate, **{
+                    '[READ].Operations':'sum',
+                    '[READ].AverageLatency(us)':'mean',
+                    '[READ].MinLatency(us)':'min',
+                    '[READ].MaxLatency(us)':'max',
+                    '[READ].95thPercentileLatency(us)':'mean',
+                    '[READ].99thPercentileLatency(us)':'mean',
+                    '[READ].Return=OK': 'sum',
+                }}
+            if '[INSERT].Operations' in grp.columns:
+                aggregate = {**aggregate, **{
+                    '[INSERT].Operations':'sum',
+                    '[INSERT].AverageLatency(us)':'mean',
+                    '[INSERT].MinLatency(us)':'min',
+                    '[INSERT].MaxLatency(us)':'max',
+                    '[INSERT].95thPercentileLatency(us)':'mean',
+                    '[INSERT].99thPercentileLatency(us)':'mean',
+                    '[INSERT].Return=OK': 'sum',
+                }}
+            if '[UPDATE].Operations' in grp.columns:
+                aggregate = {**aggregate, **{
+                    '[UPDATE].Operations':'sum',
+                    '[UPDATE].AverageLatency(us)':'mean',
+                    '[UPDATE].MinLatency(us)':'min',
+                    '[UPDATE].MaxLatency(us)':'max',
+                    '[UPDATE].95thPercentileLatency(us)':'mean',
+                    '[UPDATE].99thPercentileLatency(us)':'mean',
+                    '[UPDATE].Return=OK': 'sum',
+                }}
+            if '[SCAN].Operations' in grp.columns:
+                aggregate = {**aggregate, **{
+                    '[SCAN].Operations':'sum',
+                    '[SCAN].AverageLatency(us)':'mean',
+                    '[SCAN].MinLatency(us)':'min',
+                    '[SCAN].MaxLatency(us)':'max',
+                    '[SCAN].95thPercentileLatency(us)':'mean',
+                    '[SCAN].99thPercentileLatency(us)':'mean',
+                    '[SCAN].Return=OK':'sum',
+                }}
             #print(grp.agg(aggregate))
             dict_grp = dict()
             dict_grp['connection'] = key
             dict_grp['configuration'] = grp['configuration'][0]
             dict_grp['experiment_run'] = grp['experiment_run'][0]
             #dict_grp['client'] = grp['client'][0]
             #dict_grp['pod'] = grp['pod'][0]
@@ -578,25 +641,26 @@
             'client':'int',
             'pod':'str',
             'pod_count':'int',
             'threads':'int',
             'target':'int',
             'sf':'int',
             'workload':'str',
+            'operations':'int',
             '[OVERALL].RunTime(ms)':'float',
             '[OVERALL].Throughput(ops/sec)':'float',
-            '[TOTAL_GCS_PS_Scavenge].Count':'int',
-            '[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'float',
-            '[TOTAL_GCS_PS_MarkSweep].Count':'float',
-            '[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'float',
-            '[TOTAL_GCs].Count':'int',
-            '[TOTAL_GC_TIME].Time(ms)':'float',
-            '[TOTAL_GC_TIME_%].Time(%)':'float',
+            #'[TOTAL_GCS_PS_Scavenge].Count':'int',
+            #'[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'float',
+            #'[TOTAL_GCS_PS_MarkSweep].Count':'float',
+            #'[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'float',
+            #'[TOTAL_GCs].Count':'int',
+            #'[TOTAL_GC_TIME].Time(ms)':'float',
+            #'[TOTAL_GC_TIME_%].Time(%)':'float',
             '[CLEANUP].Operations':'int',
             '[CLEANUP].AverageLatency(us)':'float',
             '[CLEANUP].MinLatency(us)':'float',
             '[CLEANUP].MaxLatency(us)':'float',
             '[CLEANUP].95thPercentileLatency(us)':'float',
             '[CLEANUP].99thPercentileLatency(us)':'float',
             '[INSERT].Operations':'int',
@@ -625,37 +689,38 @@
                 'client':'max',
                 'pod':'sum',
                 'pod_count':'count',
                 'threads':'sum',
                 'target':'sum',
                 'sf':'max',
                 'workload':'max',
+                'operations':'sum',
                 '[OVERALL].RunTime(ms)':'max',
                 '[OVERALL].Throughput(ops/sec)':'sum',
-                '[TOTAL_GCS_PS_Scavenge].Count':'sum',
-                '[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'max',
-                '[TOTAL_GCS_PS_MarkSweep].Count':'sum',
-                '[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'max',
-                '[TOTAL_GCs].Count':'sum',
-                '[TOTAL_GC_TIME].Time(ms)':'max',
-                '[TOTAL_GC_TIME_%].Time(%)':'max',
+                #'[TOTAL_GCS_PS_Scavenge].Count':'sum',
+                #'[TOTAL_GC_TIME_PS_Scavenge].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%_PS_Scavenge].Time(%)':'max',
+                #'[TOTAL_GCS_PS_MarkSweep].Count':'sum',
+                #'[TOTAL_GC_TIME_PS_MarkSweep].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%_PS_MarkSweep].Time(%)':'max',
+                #'[TOTAL_GCs].Count':'sum',
+                #'[TOTAL_GC_TIME].Time(ms)':'max',
+                #'[TOTAL_GC_TIME_%].Time(%)':'max',
                 '[CLEANUP].Operations':'sum',
                 '[CLEANUP].AverageLatency(us)':'mean',
                 '[CLEANUP].MinLatency(us)':'min',
                 '[CLEANUP].MaxLatency(us)':'max',
-                '[CLEANUP].95thPercentileLatency(us)':'max',
-                '[CLEANUP].99thPercentileLatency(us)':'max',
+                '[CLEANUP].95thPercentileLatency(us)':'mean',
+                '[CLEANUP].99thPercentileLatency(us)':'mean',
                 '[INSERT].Operations':'sum',
                 '[INSERT].AverageLatency(us)':'mean',
                 '[INSERT].MinLatency(us)':'min',
                 '[INSERT].MaxLatency(us)':'max',
-                '[INSERT].95thPercentileLatency(us)':'max',
-                '[INSERT].99thPercentileLatency(us)':'max',
+                '[INSERT].95thPercentileLatency(us)':'mean',
+                '[INSERT].99thPercentileLatency(us)':'mean',
                 '[INSERT].Return=OK':'sum',
             }
             #print(grp.agg(aggregate))
             dict_grp = dict()
             dict_grp['connection'] = key[0]
             dict_grp['configuration'] = grp['configuration'][0]
             dict_grp['experiment_run'] = grp['experiment_run'][0]
@@ -687,20 +752,22 @@
         """
         Transforms a log file in text format into a pandas DataFrame.
 
         :param filename: Name of the log file 
         :return: DataFrame of results
         """
         stdout = ""
+        df_header = pd.DataFrame()
         try:
             with open(filename) as f:
                 lines = f.readlines()
             stdout = "".join(lines)
             pod_name = filename[filename.rindex("-")+1:-len(".log")]
             connection_name = re.findall('BEXHOMA_CONNECTION:(.+?)\n', stdout)[0]
+            duration = re.findall('BEXHOMA_DURATION:(.+?)\n', stdout)[0]
             configuration_name = re.findall('BEXHOMA_CONFIGURATION:(.+?)\n', stdout)[0]
             experiment_run = re.findall('BEXHOMA_EXPERIMENT_RUN:(.+?)\n', stdout)[0]
             client = re.findall('BEXHOMA_CLIENT:(.+?)\n', stdout)[0]
             error_timesynch = re.findall('start time has already passed', stdout)
             if len(error_timesynch) > 0:
                 # log is incomplete
                 return pd.DataFrame()
@@ -725,47 +792,49 @@
                 'profile': profile,
                 'target': target,
                 'time': time,
                 #'terminals': terminals,
                 'batchsize': batchsize,
                 'sf': sf,
                 'num_errors': num_errors,
+                'duration': duration,
             }
             df_header = pd.DataFrame(header, index=[0])
             if num_errors == 0:
                 log = re.findall('####BEXHOMA####(.+?)####BEXHOMA####', stdout, re.DOTALL)
                 if len(log) > 0:
                     result = json.loads(log[0])
                     df = pd.json_normalize(result)
                     #self.cluster.logger.debug(df)
                     df = pd.concat([df_header, df], axis=1)
                     df.index.name = connection_name
                     #print(df)
                     return df
                 else:
                     print("no results found in log file {}".format(filename))
-                    return pd.DataFrame()
+                    return df_header
             else:
-                return pd.DataFrame()
+                return df_header#pd.DataFrame()
         except Exception as e:
             print(e)
             print(traceback.format_exc())
             print(stdout)
-            return pd.DataFrame()
+            return df_header
     def benchmarking_set_datatypes(self, df):
         """
         Transforms a pandas DataFrame collection of benchmarking results to suitable data types.
 
         :param df: DataFrame of results 
         :return: DataFrame of results
         """
         df_typed = df.astype({
             'connection':'str',
             'configuration':'str',
             'experiment_run':'int',
+            'duration':'int',
             'client':'int',
             'pod':'str',
             'pod_count':'int',
             'bench':'str',
             'profile':'str',
             'target':'int',
             'time':'float',
@@ -806,14 +875,15 @@
         for key, grp in df.groupby(column):
             #print(key, len(grp.index))
             #print(grp.columns)
             aggregate = {
                 'client':'max',
                 'pod':'sum',
                 'pod_count':'count',
+                'duration':'max',
                 'bench':'max',
                 'profile':'max',
                 'target':'sum',
                 'time':'max',
                 #'terminals':'sum',
                 'batchsize':'mean',
                 'sf':'max',
@@ -991,16 +1061,19 @@
                 'iterations':'max',
                 'duration':'max',
                 'sf':'max',
                 'run':'max',
                 'errors':'max',
                 'vusers_loading':'max',
                 'vusers':'sum',
-                'NOPM':'sum',
-                'TPM':'sum',
+                #'vusers':'max',
+                #'NOPM':'sum',
+                'NOPM':'mean',
+                #'TPM':'sum',
+                'TPM':'mean',
                 'dbms':'max',
             }
             #print(grp.agg(aggregate))
             dict_grp = dict()
             dict_grp['connection'] = key[0]
             dict_grp['configuration'] = grp['configuration'][0]
             dict_grp['experiment_run'] = grp['experiment_run'][0]
```

### Comparing `bexhoma-0.6.3/bexhoma/experiments.py` & `bexhoma-0.6.4/bexhoma/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         self.benchmarking_parameters = {}
         self.jobtemplate_maintaining = ""
         self.jobtemplate_loading = ""
         self.querymanagement = {}
         self.additional_labels = dict()
         self.workload = {}
         self.monitoring_active = True
-        self.prometheus_interval = "3s"
-        self.prometheus_timeout = "3s"
+        self.prometheus_interval = "10s"
+        self.prometheus_timeout = "10s"
         self.loading_active = False
         self.num_loading = 0
         self.num_loading_pods = 0
         self.maintaining_active = False
         self.num_maintaining = 0
         self.num_maintaining_pods = 0
         self.name_format = None
@@ -753,19 +753,20 @@
                     continue
                 # check if loading is done
                 config.check_load_data()
                 # start loading
                 if not config.loading_started:
                     if config.sut_is_running():
                         print("{} is not loaded yet".format(config.configuration))
-                    if config.monitoring_active and not config.monitoring_is_running():
-                        print("{} waits for monitoring".format(config.configuration))
-                        if not config.monitoring_is_pending():
-                            config.start_monitoring()
-                        continue
+                    if len(config.benchmark_list) > 0:
+                        if config.monitoring_active and not config.monitoring_is_running():
+                            print("{} waits for monitoring".format(config.configuration))
+                            if not config.monitoring_is_pending():
+                                config.start_monitoring()
+                            continue
                     now = datetime.utcnow()
                     if config.loading_after_time is not None:
                         if now >= config.loading_after_time:
                             if config.loading_active:
                                 config.start_loading()
                                 config.start_loading_pod(parallelism=config.num_loading, num_pods=config.num_loading_pods)
                             else:
@@ -778,37 +779,39 @@
                         if 'delay_prepare' in config.dockertemplate:
                             # config demands other delay
                             delay = config.dockertemplate['delay_prepare']
                         config.loading_after_time = now + timedelta(seconds=delay)
                         print("{} will start loading but not before {} (that is in {} secs)".format(config.configuration, config.loading_after_time.strftime('%Y-%m-%d %H:%M:%S'), delay))
                         continue
                 # check if maintaining
-                if config.loading_finished:
+                if config.loading_finished and len(config.benchmark_list) > 0:
                     if config.monitoring_active and not config.monitoring_is_running():
                         print("{} waits for monitoring".format(config.configuration))
                         if not config.monitoring_is_pending():
                             config.start_monitoring()
                         continue
                     if config.maintaining_active:
                         if not config.maintaining_is_running():
                             print("{} is not maintained yet".format(config.configuration))
                             if not config.maintaining_is_pending():
                                 config.start_maintaining(parallelism=config.num_maintaining, num_pods=config.num_maintaining_pods)
                             else:
                                 print("{} has pending maintaining".format(config.configuration))
                 # start benchmarking, if loading is done and monitoring is ready
                 if config.loading_finished:
-                    if config.monitoring_active and not config.monitoring_is_running():
-                        print("{} waits for monitoring".format(config.configuration))
-                        if not config.monitoring_is_pending():
-                            config.start_monitoring()
-                        continue
-                    if config.maintaining_active and not config.maintaining_is_running():
-                        print("{} waits for maintaining".format(config.configuration))
-                        continue
+                    # still benchmarks: check loading and maintaining
+                    if len(config.benchmark_list) > 0:
+                        if config.monitoring_active and not config.monitoring_is_running():
+                            print("{} waits for monitoring".format(config.configuration))
+                            if not config.monitoring_is_pending():
+                                config.start_monitoring()
+                            continue
+                        if config.maintaining_active and not config.maintaining_is_running():
+                            print("{} waits for maintaining".format(config.configuration))
+                            continue
                     app = self.cluster.appname
                     component = 'benchmarker'
                     configuration = ''
                     pods = self.cluster.get_job_pods(app, component, self.code, configuration=config.configuration)
                     if len(pods) > 0:
                         # still pods there
                         print("{} has running benchmarks".format(config.configuration))
@@ -816,14 +819,18 @@
                     else:
                         if len(config.benchmark_list) > 0:
                             # next element in list
                             parallelism = config.benchmark_list.pop(0)
                             client = str(config.client)
                             config.client = config.client+1
                             print("Done {} of {} benchmarks. This will be client {}".format(config.num_experiment_to_apply_done, config.num_experiment_to_apply, client))
+                            if len(config.benchmarking_parameters_list) > 0:
+                                benchmarking_parameters = config.benchmarking_parameters_list.pop(0)
+                                print("We will change parameters of benchmark", benchmarking_parameters)
+                                config.set_benchmarking_parameters(**benchmarking_parameters)
                             if config.num_experiment_to_apply > 1:
                                 connection=config.configuration+'-'+str(config.num_experiment_to_apply_done+1)+'-'+client
                             else:
                                 connection=config.configuration+'-'+client
                             print("Running benchmark {}".format(connection))
                             config.run_benchmarker_pod(connection=connection, configuration=config.configuration, client=client, parallelism=parallelism)
                             #config.run_benchmarker_pod_hammerdb(connection=connection, configuration=config.configuration, client=client, parallelism=parallelism)
@@ -864,29 +871,46 @@
             configuration = ''
             #success = self.cluster.get_job_status(app=app, component=component, experiment=self.code, configuration=configuration)
             jobs = self.cluster.get_jobs(app, component, self.code, configuration)
             # all pods to these jobs
             pods = self.cluster.get_job_pods(app, component, self.code, configuration)
             # status per job
             for job in jobs:
+                # status per pod
+                for p in pods:
+                    status = self.cluster.get_pod_status(p)
+                    self.cluster.logger.debug('job-pod {} has status {}'.format(p, status))
+                    #print(p,status)
+                    if status == 'Succeeded':
+                        print("Store logs of job {} pod {}".format(job, p))
+                        #if status != 'Running':
+                        self.cluster.store_pod_log(p)
+                        #self.cluster.delete_pod(p)
+                    if status == 'Failed':
+                        print("Store logs of job {} pod {}".format(job, p))
+                        #if status != 'Running':
+                        self.cluster.store_pod_log(p)
+                        #self.cluster.delete_pod(p)
                 success = self.cluster.get_job_status(job)
                 self.cluster.logger.debug('job {} has success status {}'.format(job, success))
                 #print(job, success)
                 if success:
                     # status per pod
                     for p in pods:
                         status = self.cluster.get_pod_status(p)
                         self.cluster.logger.debug('job-pod {} has status {}'.format(p, status))
                         #print(p,status)
                         if status == 'Succeeded':
                             #if status != 'Running':
+                            print("Store logs of job {} pod {}".format(job, p))
                             self.cluster.store_pod_log(p)
                             self.cluster.delete_pod(p)
                         if status == 'Failed':
                             #if status != 'Running':
+                            print("Store logs of job {} pod {}".format(job, p))
                             self.cluster.store_pod_log(p)
                             self.cluster.delete_pod(p)
                     self.end_benchmarking(job, config)
                     self.cluster.delete_job(job)
             if len(pods) == 0 and len(jobs) == 0:
                 do = False
                 for config in self.configurations:
@@ -1052,14 +1076,28 @@
                     self.cluster.logger.debug(stdout)
                     self.cluster.logger.debug(stderr)
                     # upload connections infos again, metrics has overwritten it
                     filename = 'connections.config'
                     cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
                     stdout = self.cluster.kubectl(cmd['upload_connection_file'])
                     self.cluster.logger.debug(stdout)
+                    # get metrics of benchmarker components
+                    # only if general monitoring is on
+                    endpoints_cluster = self.cluster.get_service_endpoints(service_name="bexhoma-service-monitoring-default")
+                    if len(endpoints_cluster)>0:
+                        cmd['fetch_benchmarker_metrics'] = 'python metrics.py -r /results/ -db -ct benchmarker -cn dbmsbenchmarker -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(connection, connection+'.config', '/results/'+self.code, self.code, start_time, end_time)
+                        #cmd['fetch_loading_metrics'] = 'python metrics.py -r /results/ -db -ct loading -c {} -cf {} -f {} -e {} -ts {} -te {}'.format(connection, c['name']+'.config', '/results/'+self.code, self.code, self.timeLoadingStart, self.timeLoadingEnd)
+                        stdin, stdout, stderr = self.cluster.execute_command_in_pod(command=cmd['fetch_benchmarker_metrics'], pod=pod_dashboard, container="dashboard")
+                        self.cluster.logger.debug(stdout)
+                        self.cluster.logger.debug(stderr)
+                        # upload connections infos again, metrics has overwritten it
+                        filename = 'connections.config'
+                        cmd['upload_connection_file'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/'+filename, from_file=self.path+"/"+filename)
+                        stdout = self.cluster.kubectl(cmd['upload_connection_file'])
+                        self.cluster.logger.debug(stdout)
         self.evaluator.end_benchmarking(jobname)
     def end_loading(self, jobname):
         """
         Ends a loading job.
         This is for storing or cleaning measures.
 
         :param jobname: Name of the job to clean
@@ -1139,19 +1177,22 @@
     def __init__(self,
             cluster,
             code=None,
             queryfile = 'queries-tpch.config',
             SF = '100',
             num_experiment_to_apply = 1,
             timeout = 7200,
+            script=None
             #detached=False
             ):
         default.__init__(self, cluster, code, num_experiment_to_apply, timeout)#, detached)
+        if script is None:
+            script = 'SF'+str(SF)+'-index'
         self.set_experiment(volume='tpch')
-        self.set_experiment(script='SF'+str(SF)+'-index')
+        self.set_experiment(script=script)
         self.cluster.set_experiments_configfolder('experiments/tpch')
         parameter.defaultParameters = {'SF': str(SF)}
         self.set_additional_labels(SF=SF)
         self.set_queryfile(queryfile)
         self.set_workload(
             name = 'TPC-H Queries SF='+str(SF),
             info = 'This experiment performs some TPC-H inspired queries.'
@@ -1259,14 +1300,17 @@
         #cmd['evaluate_results'] = 'python benchmark.py read -e yes -r /results/'+str(self.code)
         #self.cluster.execute_command_in_pod(command=cmd['evaluate_results'], pod=pod_dashboard, container="dashboard")
         #print("done!")
         # download all results from cluster
         #filename = 'evaluation.json'
         cmd['download_results'] = 'cp {from_file} {to} -c dashboard'.format(from_file=pod_dashboard+':/results/'+str(self.code)+'/', to=self.path+"/")
         self.cluster.kubectl(cmd['download_results'])
+        cmd['upload_results'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/', from_file=self.path+"/")
+        #cmd['upload_results'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/', from_file=self.path+"/")
+        self.cluster.kubectl(cmd['upload_results'])
 
 
 
 """
 ############################################################################
 Simple IoT example experiment
 ############################################################################
@@ -1412,15 +1456,15 @@
         self.set_workload(
             name = 'YCSB Queries SF='+str(SF),
             info = 'This experiment performs some YCSB inspired workloads.'
             )
         self.storage_label = 'tpch-'+str(SF)
         self.jobtemplate_loading = "jobtemplate-loading-ycsb.yml"
         self.evaluator = evaluators.ycsb(code=self.code, path=self.cluster.resultfolder, include_loading=False, include_benchmarking=True)
-    def log_to_df(self, filename):
+    def OLD_log_to_df(self, filename):
         try:
             with open(filename) as f:
                 lines = f.readlines()
             stdout = "".join(lines)
             connection_name = re.findall('BEXHOMA_CONNECTION:(.+?)\n', stdout)
             result = []
             #for line in s.split("\n"):
@@ -1448,49 +1492,49 @@
         self.cluster.logger.debug('ycsb.test_results()')
         self.evaluator.test_results()
         workflow = self.get_workflow_list()
         if workflow == self.evaluator.workflow:
             print("Result workflow complete")
         else:
             print("Result workflow not complete")
-    def get_result_sum(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
+    def OLD_get_result_sum(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
         try:
             df2=df[df['type'] == type]
             s=df2[df2['category'] == category]
             total = s.drop(columns=['category','type']).apply(pd.to_numeric).sum(axis=1)
             return total.iloc[0]
         except Exception as e:
             print(e)
             print(df)
             return 0.0
-    def get_result_max(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
+    def OLD_get_result_max(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
         try:
             df2=df[df['type'] == type]
             s=df2[df2['category'] == category]
             total = s.drop(columns=['category','type']).apply(pd.to_numeric).max(axis=1)
             return total.iloc[0]
         except Exception as e:
             print(e)
             print(df)
             return 0.0
-    def get_result_avg(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
+    def OLD_get_result_avg(self, df, category='[OVERALL]', type='Throughput(ops/sec)'):
         try:
             df2=df[df['type'] == type]
             s=df2[df2['category'] == category]
             total = s.drop(columns=['category','type']).apply(pd.to_numeric).mean(axis=1)
             return total.iloc[0]
         except Exception as e:
             print(e)
             print(df)
             return 0.0
-    def get_parts_of_name(self, name):
+    def OLD_get_parts_of_name(self, name):
         parts_name = re.findall('{(.+?)}', self.name_format)
         parts_values = re.findall('-(.+?)-', "-"+name.replace("-","--")+"--")
         return dict(zip(parts_name, parts_values))
-    def get_overview_loading(self, dfs={}):
+    def OLD_get_overview_loading(self, dfs={}):
         tps = []
         if len(dfs) == 0:
             dfs = self.get_result(component="loading")
         for connection, df in dfs.items():
             #print(connection)
             if df.empty:
                 print(connection, "is empty")
@@ -1508,32 +1552,54 @@
             overall_RunTime = float(self.get_result_max(df, category='[OVERALL]', type='RunTime(ms)'))
             insert_AverageLatency = float(self.get_result_avg(df, category='[INSERT]', type='AverageLatency(us)'))
             insert_95thPercentileLatency = float(self.get_result_avg(df, category='[INSERT]', type='95thPercentileLatency(us)'))
             insert_99thPercentileLatency = float(self.get_result_avg(df, category='[INSERT]', type='99thPercentileLatency(us)'))
             list_values_name = list(parts.values())
             num_pods = len(df.columns)-2
             #print(list_values_name)
-            list_values_df = [connection, num_pods, overall_Throughput, insert_Operations, insert_OK, overall_RunTime, insert_AverageLatency, insert_95thPercentileLatency, insert_99thPercentileLatency, overall_Throughput/int(parts['pods'])]
+            list_values_df = [
+                connection, 
+                num_pods, 
+                overall_Throughput/int(parts['pods']),
+                overall_Throughput, 
+                overall_RunTime, 
+                insert_Operations, 
+                insert_OK, 
+                insert_AverageLatency, 
+                insert_95thPercentileLatency, 
+                insert_99thPercentileLatency, 
+                ]
             #print(list_values_df)
             list_values_name.extend(list_values_df)
             #print('combined', list_values_name)
             tps.append(list_values_name)
             #print(target, worker, pods, overall_Throughput, overall_RunTime, overall_Throughput, total_tps/pods)
         #print(tps)
         df_totals = pd.DataFrame(tps)
         #print(list(parts.keys()))
         columns = list(parts.keys())
-        columns.extend(['connection', 'num_pods', 'overall_Throughput', 'insert_Operations', 'insert_OK', 'overall_RunTime', 'insert_AverageLatency', 'insert_95thPercentileLatency', 'insert_99thPercentileLatency', 'total_tps_per_pod'])
+        columns.extend([
+            'connection', 
+            'num_pods', 
+            'total_tps_per_pod', 
+            'overall_Throughput', 
+            'overall_RunTime', 
+            'insert_Operations', 
+            'insert_OK', 
+            'insert_AverageLatency', 
+            'insert_95thPercentileLatency', 
+            'insert_99thPercentileLatency',
+            ])
         #print(columns)
         df_totals.columns = columns
         #list(parts.keys()).extend(['overall_Throughput', 'insert_Operations', 'insert_OK', 'overall_RunTime', 'insert_AverageLatency', 'insert_95thPercentileLatency', 'insert_99thPercentileLatency', 'total_tps_per_pod'])
         df_totals = df_totals.astype({'target':'float','pods':'int'})
         df_totals = df_totals.sort_values(['target','pods'])
         return df_totals
-    def get_overview_benchmarking(self, dfs={}):
+    def OLD_get_overview_benchmarking(self, dfs={}):
         tps = []
         if len(dfs) == 0:
             dfs = self.get_result(component="benchmarking")
         for connection, df in dfs.items():
             #print(connection)
             if df.empty:
                 print(connection, "is empty")
@@ -1542,45 +1608,109 @@
             #parts = re.findall('-(.+?)-', connection.replace("-","--")+"--")
             #print(parts)
             #threads = int(parts[1])
             #pods = int(parts[1])
             #worker = int(parts[2])
             #target = int(parts[3])
             #print(df)
+            # read
             read_Operations = float(self.get_result_sum(df, category='[READ]', type='Operations'))
             read_OK = float(self.get_result_sum(df, category='[READ]', type='Return=OK'))
             read_AverageLatency = float(self.get_result_avg(df, category='[READ]', type='AverageLatency(us)'))
             read_95thPercentileLatency = float(self.get_result_avg(df, category='[READ]', type='95thPercentileLatency(us)'))
             read_99thPercentileLatency = float(self.get_result_avg(df, category='[READ]', type='99thPercentileLatency(us)'))
+            # update
             update_Operations = float(self.get_result_sum(df, category='[UPDATE]', type='Operations'))
             update_OK = float(self.get_result_sum(df, category='[UPDATE]', type='Return=OK'))
             update_AverageLatency = float(self.get_result_avg(df, category='[UPDATE]', type='AverageLatency(us)'))
             update_95thPercentileLatency = float(self.get_result_avg(df, category='[UPDATE]', type='95thPercentileLatency(us)'))
             update_99thPercentileLatency = float(self.get_result_avg(df, category='[UPDATE]', type='99thPercentileLatency(us)'))
+            # overall
             overall_Throughput = float(self.get_result_sum(df, category='[OVERALL]', type='Throughput(ops/sec)'))
             overall_RunTime = float(self.get_result_max(df, category='[OVERALL]', type='RunTime(ms)'))
+            # inserts
+            insert_Operations = float(self.get_result_sum(df, category='[INSERT]', type='Operations'))
+            insert_OK = float(self.get_result_sum(df, category='[INSERT]', type='Return=OK'))
+            insert_AverageLatency = float(self.get_result_avg(df, category='[INSERT]', type='AverageLatency(us)'))
+            insert_95thPercentileLatency = float(self.get_result_avg(df, category='[INSERT]', type='95thPercentileLatency(us)'))
+            insert_99thPercentileLatency = float(self.get_result_avg(df, category='[INSERT]', type='99thPercentileLatency(us)'))
+            # scan
+            scan_Operations = float(self.get_result_sum(df, category='[SCAN]', type='Operations'))
+            scan_OK = float(self.get_result_sum(df, category='[SCAN]', type='Return=OK'))
+            scan_AverageLatency = float(self.get_result_avg(df, category='[SCAN]', type='AverageLatency(us)'))
+            scan_95thPercentileLatency = float(self.get_result_avg(df, category='[SCAN]', type='95thPercentileLatency(us)'))
+            scan_99thPercentileLatency = float(self.get_result_avg(df, category='[SCAN]', type='99thPercentileLatency(us)'))
+            # extract from naming (DEPRCATED?)
             list_values_name = list(parts.values())
             num_pods = len(df.columns)-2
             #print(list_values_name)
-            list_values_df = [connection, num_pods, overall_Throughput, overall_RunTime, read_Operations, read_OK, read_AverageLatency, read_95thPercentileLatency, read_99thPercentileLatency,
-                        update_Operations, update_OK, update_AverageLatency, update_95thPercentileLatency, update_99thPercentileLatency, overall_Throughput/int(parts['pods'])]
+            list_values_df = [
+                connection, 
+                num_pods, 
+                overall_Throughput, 
+                overall_RunTime, 
+                overall_Throughput/int(parts['pods']),
+                read_Operations, 
+                read_OK, 
+                read_AverageLatency, 
+                read_95thPercentileLatency, 
+                read_99thPercentileLatency, 
+                update_Operations, 
+                update_OK, 
+                update_AverageLatency, 
+                update_95thPercentileLatency, 
+                update_99thPercentileLatency, 
+                insert_Operations, 
+                insert_OK, 
+                insert_AverageLatency, 
+                insert_95thPercentileLatency, 
+                insert_99thPercentileLatency, 
+                scan_Operations, 
+                scan_OK, 
+                scan_AverageLatency, 
+                scan_95thPercentileLatency, 
+                scan_99thPercentileLatency, 
+                ]
             #print(list_values_df)
             list_values_name.extend(list_values_df)
             #print('combined', list_values_name)
             tps.append(list_values_name)
             #tps.append(list(parts.values()).extend([target, worker, pods, overall_Throughput, overall_RunTime, read_Operations, read_OK, read_AverageLatency, read_95thPercentileLatency, read_99thPercentileLatency,
             #            update_Operations, update_OK, update_AverageLatency, update_95thPercentileLatency, update_99thPercentileLatency, overall_Throughput/pods]))
             #print(target, worker, pods, overall_Throughput, overall_RunTime, overall_Throughput, total_tps/pods)
         #print(tps)
         df_totals = pd.DataFrame(tps)
         columns = list(parts.keys())
-        columns.extend(['connection', 'num_pods', 'overall_Throughput', 'overall_RunTime', 
-                             'read_Operations', 'read_OK', 'read_AverageLatency', 'read_95thPercentileLatency', 'read_99thPercentileLatency',
-                             'update_Operations', 'update_OK', 'update_AverageLatency', 'update_95thPercentileLatency', 'update_99thPercentileLatency',
-                             'total_tps_per_pod'])
+        columns.extend([
+            'connection', 
+            'num_pods', 
+            'overall_Throughput', 
+            'overall_RunTime', 
+            'total_tps_per_pod',
+            'read_Operations', 
+            'read_OK', 
+            'read_AverageLatency', 
+            'read_95thPercentileLatency', 
+            'read_99thPercentileLatency', 
+            'update_Operations', 
+            'update_OK', 
+            'update_AverageLatency', 
+            'update_95thPercentileLatency', 
+            'update_99thPercentileLatency', 
+            'insert_Operations', 
+            'insert_OK', 
+            'insert_AverageLatency', 
+            'insert_95thPercentileLatency', 
+            'insert_99thPercentileLatency'
+            'scan_Operations', 
+            'scan_OK', 
+            'scan_AverageLatency', 
+            'scan_95thPercentileLatency', 
+            'scan_99thPercentileLatency',
+            ])
         #print(columns)
         df_totals.columns = columns
         df_totals = df_totals.astype({'target':'float','pods':'int'})
         df_totals = df_totals.sort_values(['target','pods'])
         return df_totals
     def evaluate_results(self, pod_dashboard=''):
         """
@@ -1605,17 +1735,24 @@
             cmd['transform_benchmarking_metrics'] = 'python metrics.evaluation.py -r /results/ -db -ct loading -e {}'.format(self.code)
             stdin, stdout, stderr = self.cluster.execute_command_in_pod(command=cmd['transform_benchmarking_metrics'], pod=pod_dashboard, container="dashboard")
             self.cluster.logger.debug(stdout)
             cmd['transform_benchmarking_metrics'] = 'python metrics.evaluation.py -r /results/ -db -ct stream -e {}'.format(self.code)
             stdin, stdout, stderr = self.cluster.execute_command_in_pod(command=cmd['transform_benchmarking_metrics'], pod=pod_dashboard, container="dashboard")
             self.cluster.logger.debug(stdout)
         cmd = {}
+        #stdout = self.experiment.cluster.kubectl('cp --container dashboard '+self.path+'/connections.config '+pod_dashboard+':/results/'+str(self.code)+'/connections.config')
+        #self.logger.debug('copy config connections.config: {}'.format(stdout))
+        #cmd['upload_config'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/connections.config', from_file=self.path+"/connections.config")
+        #self.cluster.kubectl(cmd['upload_config'])
         cmd['download_results'] = 'cp {from_file} {to} -c dashboard'.format(from_file=pod_dashboard+':/results/'+str(self.code)+'/', to=self.path+"/")
         self.cluster.kubectl(cmd['download_results'])
-    def get_result(self, component='loading'):
+        cmd['upload_results'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/', from_file=self.path+"/")
+        #cmd['upload_results'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/'+str(self.code)+'/', from_file=self.path+"/")
+        self.cluster.kubectl(cmd['upload_results'])
+    def OLD_get_result(self, component='loading'):
         #path = self.cluster.config['benchmarker']['resultfolder'].replace("\\", "/").replace("C:", "")+'/{}'.format(self.code)
         path = self.path
         df_prev = pd.DataFrame()
         #pod_numbers = {}
         if component == "loading":
             ending = "sensor.log"
         else:
@@ -1780,9 +1917,11 @@
             self.cluster.logger.debug(stdout)
             cmd['transform_benchmarking_metrics'] = 'python metrics.evaluation.py -r /results/ -db -ct stream -e {}'.format(self.code)
             stdin, stdout, stderr = self.cluster.execute_command_in_pod(command=cmd['transform_benchmarking_metrics'], pod=pod_dashboard, container="dashboard")
             self.cluster.logger.debug(stdout)
         cmd = {}
         cmd['download_results'] = 'cp {from_file} {to} -c dashboard'.format(from_file=pod_dashboard+':/results/'+str(self.code)+'/', to=self.path+"/")
         self.cluster.kubectl(cmd['download_results'])
+        cmd['upload_results'] = 'cp {from_file} {to} -c dashboard'.format(to=pod_dashboard+':/results/', from_file=self.path+"/")
+        self.cluster.kubectl(cmd['upload_results'])
```

### Comparing `bexhoma-0.6.3/bexhoma/scripts/experimentsmanager.py` & `bexhoma-0.6.4/bexhoma/scripts/experimentsmanager.py`

 * *Files identical despite different names*

### Comparing `bexhoma-0.6.3/bexhoma/scripts/tpcds.py` & `bexhoma-0.6.4/bexhoma/scripts/tpcds.py`

 * *Files identical despite different names*

### Comparing `bexhoma-0.6.3/bexhoma/scripts/tpch.py` & `bexhoma-0.6.4/bexhoma/scripts/tpch.py`

 * *Files identical despite different names*

### Comparing `bexhoma-0.6.3/bexhoma.egg-info/PKG-INFO` & `bexhoma-0.6.4/bexhoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bexhoma
-Version: 0.6.3
+Version: 0.6.4
 Summary: This python tools helps managing DBMS benchmarking experiments in a Kubernetes-based HPC cluster environment. It enables users to configure hardware / software setups for easily repeating tests over varying configurations.
 Home-page: https://github.com/Beuth-Erdelt/Benchmark-Experiment-Host-Manager
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `bexhoma-0.6.3/setup.py` & `bexhoma-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="bexhoma",
-    version="0.6.3",
+    version="0.6.4",
     author="Patrick Erdelt",
     author_email="perdelt@beuth-hochschule.de",
     description="This python tools helps managing DBMS benchmarking experiments in a Kubernetes-based HPC cluster environment. It enables users to configure hardware / software setups for easily repeating tests over varying configurations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Beuth-Erdelt/Benchmark-Experiment-Host-Manager",
     packages=setuptools.find_packages(),
```

