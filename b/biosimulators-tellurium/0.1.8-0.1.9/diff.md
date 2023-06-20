# Comparing `tmp/biosimulators_tellurium-0.1.8.tar.gz` & `tmp/biosimulators_tellurium-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosimulators_tellurium-0.1.8.tar", last modified: Mon May  3 23:40:14 2021, max compression
+gzip compressed data, was "biosimulators_tellurium-0.1.9.tar", last modified: Sat Jun  5 06:47:30 2021, max compression
```

## Comparing `biosimulators_tellurium-0.1.8.tar` & `biosimulators_tellurium-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 23:40:14.069069 biosimulators_tellurium-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2021-05-03 23:40:14.069069 biosimulators_tellurium-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-05-03 23:40:07.000000 biosimulators_tellurium-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 23:40:14.069069 biosimulators_tellurium-0.1.8/biosimulators_tellurium/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8901 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 23:40:14.069069 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-03 23:40:13.000000 biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/requirements.optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-03 23:40:14.069069 biosimulators_tellurium-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2021-05-03 23:36:47.000000 biosimulators_tellurium-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-05 06:47:30.705175 biosimulators_tellurium-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4662 2021-06-05 06:47:30.705175 biosimulators_tellurium-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-06-05 06:47:25.000000 biosimulators_tellurium-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-05 06:47:30.705175 biosimulators_tellurium-0.1.9/biosimulators_tellurium/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9081 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-05 06:47:30.705175 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4662 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-06-05 06:47:30.000000 biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/requirements.optional.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-06-05 06:47:30.705175 biosimulators_tellurium-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2033 2021-06-05 06:44:28.000000 biosimulators_tellurium-0.1.9/setup.py
```

### Comparing `biosimulators_tellurium-0.1.8/LICENSE` & `biosimulators_tellurium-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biosimulators_tellurium-0.1.8/PKG-INFO` & `biosimulators_tellurium-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,138 @@
 Metadata-Version: 2.1
 Name: biosimulators_tellurium
-Version: 0.1.8
+Version: 0.1.9
 Summary: BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
 Home-page: https://github.com/biosimulators/Biosimulators_tellurium
 Author: BioSimulators Team
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_tellurium
-Description: |Latest release| |PyPI| |CI status| |Test coverage|
-        
-        BioSimulators-tellurium
-        =======================
-        
-        BioSimulators-compliant command-line interface and Docker image for the
-        `tellurium <http://tellurium.analogmachine.org/>`__ simulation program.
-        
-        This command-line interface and Docker image enable users to use
-        tellurium to execute `COMBINE/OMEX
-        archives <https://combinearchive.org/>`__ that describe one or more
-        simulation experiments (in `SED-ML format <https://sed-ml.org>`__) of
-        one or more models (in `SBML format <http://sbml.org]>`__).
-        
-        A list of the algorithms and algorithm parameters supported by tellurium
-        is available at
-        `BioSimulators <https://biosimulators.org/simulators/tellurium>`__.
-        
-        A simple web application and web service for using tellurium to execute
-        COMBINE/OMEX archives is also available at
-        `runBioSimulations <https://run.biosimulations.org>`__.
-        
-        Installation
-        ------------
-        
-        Install Python package
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-           pip install biosimulators-tellurium
-        
-        Install Docker image
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-           docker pull ghcr.io/biosimulators/tellurium
-        
-        Usage
-        -----
-        
-        Local usage
-        ~~~~~~~~~~~
-        
-        ::
-        
-           usage: tellurium [-h] [-d] [-q] -i ARCHIVE [-o OUT_DIR] [-v]
-        
-           BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
-        
-           optional arguments:
-             -h, --help            show this help message and exit
-             -d, --debug           full application debug mode
-             -q, --quiet           suppress all console output
-             -i ARCHIVE, --archive ARCHIVE
-                                   Path to OMEX file which contains one or more SED-ML-
-                                   encoded simulation experiments
-             -o OUT_DIR, --out-dir OUT_DIR
-                                   Directory to save outputs
-             -v, --version         show program's version number and exit
-        
-        Usage through Docker container
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The entrypoint to the Docker image supports the same command-line
-        interface described above.
-        
-        For example, the following command could be used to use the Docker image
-        to execute the COMBINE/OMEX archive ``./modeling-study.omex`` and save
-        its outputs to ``./``.
-        
-        ::
-        
-           docker run \
-             --tty \
-             --rm \
-             --mount type=bind,source="$(pwd)",target=/root/in,readonly \
-             --mount type=bind,source="$(pwd)",target=/root/out \
-             ghcr.io/biosimulators/tellurium:latest \
-               -i /root/in/modeling-study.omex \
-               -o /root/out
-        
-        Documentation
-        -------------
-        
-        Documentation is available at
-        https://biosimulators.github.io/Biosimulators_tellurium/.
-        
-        License
-        -------
-        
-        This package is released under the `MIT license <LICENSE>`__.
-        
-        Development team
-        ----------------
-        
-        This package was developed by the `Center for Reproducible Biomedical
-        Modeling <http://reproduciblebiomodels.org>`__ and the `Karr
-        Lab <https://www.karrlab.org>`__ at the Icahn School of Medicine at
-        Mount Sinai in New York.
-        
-        Questions and comments
-        ----------------------
-        
-        Please contact the `BioSimulators
-        Team <mailto:info@biosimulators.org>`__ with any questions or comments.
-        
-        .. |Latest release| image:: https://img.shields.io/github/v/tag/biosimulators/Biosimulators_tellurium
-           :target: https://github.com/biosimulations/Biosimulators_tellurium/releases
-        .. |PyPI| image:: https://img.shields.io/pypi/v/biosimulators_tellurium
-           :target: https://pypi.org/project/biosimulators_tellurium/
-        .. |CI status| image:: https://github.com/biosimulators/Biosimulators_tellurium/workflows/Continuous%20integration/badge.svg
-           :target: https://github.com/biosimulators/Biosimulators_tellurium/actions?query=workflow%3A%22Continuous+integration%22
-        .. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_tellurium/branch/dev/graph/badge.svg
-           :target: https://codecov.io/gh/biosimulators/Biosimulators_tellurium
-        
 Keywords: systems biology,computational biology,kinetic modeling,numerical simulation,stochastic,SBML,SED-ML,COMBINE,BioSimulators
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: all
+License-File: LICENSE
+
+|Latest release| |PyPI| |CI status| |Test coverage|
+
+BioSimulators-tellurium
+=======================
+
+BioSimulators-compliant command-line interface and Docker image for the
+`tellurium <http://tellurium.analogmachine.org/>`__ simulation program.
+
+This command-line interface and Docker image enable users to use
+tellurium to execute `COMBINE/OMEX
+archives <https://combinearchive.org/>`__ that describe one or more
+simulation experiments (in `SED-ML format <https://sed-ml.org>`__) of
+one or more models (in `SBML format <http://sbml.org]>`__).
+
+A list of the algorithms and algorithm parameters supported by tellurium
+is available at
+`BioSimulators <https://biosimulators.org/simulators/tellurium>`__.
+
+A simple web application and web service for using tellurium to execute
+COMBINE/OMEX archives is also available at
+`runBioSimulations <https://run.biosimulations.org>`__.
+
+Installation
+------------
+
+Install Python package
+~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+   pip install biosimulators-tellurium
+
+Install Docker image
+~~~~~~~~~~~~~~~~~~~~
+
+::
+
+   docker pull ghcr.io/biosimulators/tellurium
+
+Usage
+-----
+
+Local usage
+~~~~~~~~~~~
+
+::
+
+   usage: tellurium [-h] [-d] [-q] -i ARCHIVE [-o OUT_DIR] [-v]
+
+   BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     -d, --debug           full application debug mode
+     -q, --quiet           suppress all console output
+     -i ARCHIVE, --archive ARCHIVE
+                           Path to OMEX file which contains one or more SED-ML-
+                           encoded simulation experiments
+     -o OUT_DIR, --out-dir OUT_DIR
+                           Directory to save outputs
+     -v, --version         show program's version number and exit
+
+Usage through Docker container
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The entrypoint to the Docker image supports the same command-line
+interface described above.
+
+For example, the following command could be used to use the Docker image
+to execute the COMBINE/OMEX archive ``./modeling-study.omex`` and save
+its outputs to ``./``.
+
+::
+
+   docker run \
+     --tty \
+     --rm \
+     --mount type=bind,source="$(pwd)",target=/root/in,readonly \
+     --mount type=bind,source="$(pwd)",target=/root/out \
+     ghcr.io/biosimulators/tellurium:latest \
+       -i /root/in/modeling-study.omex \
+       -o /root/out
+
+Documentation
+-------------
+
+Documentation is available at
+https://biosimulators.github.io/Biosimulators_tellurium/.
+
+License
+-------
+
+This package is released under the `MIT license <LICENSE>`__.
+
+Development team
+----------------
+
+This package was developed by the `Center for Reproducible Biomedical
+Modeling <http://reproduciblebiomodels.org>`__ and the `Karr
+Lab <https://www.karrlab.org>`__ at the Icahn School of Medicine at
+Mount Sinai in New York.
+
+Questions and comments
+----------------------
+
+Please contact the `BioSimulators
+Team <mailto:info@biosimulators.org>`__ with any questions or comments.
+
+.. |Latest release| image:: https://img.shields.io/github/v/tag/biosimulators/Biosimulators_tellurium
+   :target: https://github.com/biosimulations/Biosimulators_tellurium/releases
+.. |PyPI| image:: https://img.shields.io/pypi/v/biosimulators_tellurium
+   :target: https://pypi.org/project/biosimulators_tellurium/
+.. |CI status| image:: https://github.com/biosimulators/Biosimulators_tellurium/workflows/Continuous%20integration/badge.svg
+   :target: https://github.com/biosimulators/Biosimulators_tellurium/actions?query=workflow%3A%22Continuous+integration%22
+.. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_tellurium/branch/dev/graph/badge.svg
+   :target: https://codecov.io/gh/biosimulators/Biosimulators_tellurium
+
+
```

### Comparing `biosimulators_tellurium-0.1.8/README.rst` & `biosimulators_tellurium-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `biosimulators_tellurium-0.1.8/biosimulators_tellurium/__main__.py` & `biosimulators_tellurium-0.1.9/biosimulators_tellurium/__main__.py`

 * *Files identical despite different names*

### Comparing `biosimulators_tellurium-0.1.8/biosimulators_tellurium/config.py` & `biosimulators_tellurium-0.1.9/biosimulators_tellurium/config.py`

 * *Files identical despite different names*

### Comparing `biosimulators_tellurium-0.1.8/biosimulators_tellurium/core.py` & `biosimulators_tellurium-0.1.9/biosimulators_tellurium/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :Date: 2021-01-04
 :Copyright: 2020-2021, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
 from .config import Config
 from biosimulators_utils.combine.exec import exec_sedml_docs_in_archive
-from biosimulators_utils.log.data_model import Status, CombineArchiveLog, SedDocumentLog  # noqa: F401
+from biosimulators_utils.log.data_model import Status, CombineArchiveLog, SedDocumentLog, StandardOutputErrorCapturerLevel  # noqa: F401
 from biosimulators_utils.plot.data_model import PlotFormat  # noqa: F401
 from biosimulators_utils.report.data_model import DataSetResults, ReportResults, ReportFormat  # noqa: F401
 from biosimulators_utils.report.io import ReportWriter
 from biosimulators_utils.sedml.data_model import Task, Report, DataSet, Plot2D, Curve, Plot3D, Surface
 from biosimulators_utils.sedml.io import SedmlSimulationReader, SedmlSimulationWriter
 from tellurium.sedml.tesedml import SEDMLCodeFactory
 import glob
@@ -58,15 +58,15 @@
         keep_individual_outputs=keep_individual_outputs,
         sed_doc_executer_logged_features=(),
     )
 
 
 def exec_sed_doc(filename, working_dir, base_out_path, rel_out_path=None,
                  apply_xml_model_changes=True, report_formats=None, plot_formats=None,
-                 log=None, indent=0):
+                 log=None, indent=0, log_level=StandardOutputErrorCapturerLevel.c):
     """
     Args:
         filename (:obj:`str`): a path to SED-ML file which defines a SED document
         working_dir (:obj:`str`): working directory of the SED document (path relative to which models are located)
 
         out_path (:obj:`str`): path to store the outputs
 
@@ -78,14 +78,15 @@
         rel_out_path (:obj:`str`, optional): path relative to :obj:`out_path` to store the outputs
         apply_xml_model_changes (:obj:`bool`, optional): if :obj:`True`, apply any model changes specified in the SED-ML file before
             calling :obj:`task_executer`.
         report_formats (:obj:`list` of :obj:`ReportFormat`, optional): report format (e.g., csv or h5)
         plot_formats (:obj:`list` of :obj:`PlotFormat`, optional): plot format (e.g., pdf)
         log (:obj:`SedDocumentLog`, optional): execution status of document
         indent (:obj:`int`, optional): degree to indent status messages
+        log_level (:obj:`StandardOutputErrorCapturerLevel`, optional): level at which to log output
 
     Returns:
         :obj:`ReportResults`: results of each report
     """
     # Set the engine that tellurium uses for plotting
     tellurium.setDefaultPlottingEngine(Config().plotting_engine.value)
```

### Comparing `biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/PKG-INFO` & `biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,138 @@
 Metadata-Version: 2.1
 Name: biosimulators-tellurium
-Version: 0.1.8
+Version: 0.1.9
 Summary: BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
 Home-page: https://github.com/biosimulators/Biosimulators_tellurium
 Author: BioSimulators Team
 Author-email: info@biosimulators.org
 License: MIT
 Download-URL: https://github.com/biosimulators/Biosimulators_tellurium
-Description: |Latest release| |PyPI| |CI status| |Test coverage|
-        
-        BioSimulators-tellurium
-        =======================
-        
-        BioSimulators-compliant command-line interface and Docker image for the
-        `tellurium <http://tellurium.analogmachine.org/>`__ simulation program.
-        
-        This command-line interface and Docker image enable users to use
-        tellurium to execute `COMBINE/OMEX
-        archives <https://combinearchive.org/>`__ that describe one or more
-        simulation experiments (in `SED-ML format <https://sed-ml.org>`__) of
-        one or more models (in `SBML format <http://sbml.org]>`__).
-        
-        A list of the algorithms and algorithm parameters supported by tellurium
-        is available at
-        `BioSimulators <https://biosimulators.org/simulators/tellurium>`__.
-        
-        A simple web application and web service for using tellurium to execute
-        COMBINE/OMEX archives is also available at
-        `runBioSimulations <https://run.biosimulations.org>`__.
-        
-        Installation
-        ------------
-        
-        Install Python package
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-           pip install biosimulators-tellurium
-        
-        Install Docker image
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-           docker pull ghcr.io/biosimulators/tellurium
-        
-        Usage
-        -----
-        
-        Local usage
-        ~~~~~~~~~~~
-        
-        ::
-        
-           usage: tellurium [-h] [-d] [-q] -i ARCHIVE [-o OUT_DIR] [-v]
-        
-           BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
-        
-           optional arguments:
-             -h, --help            show this help message and exit
-             -d, --debug           full application debug mode
-             -q, --quiet           suppress all console output
-             -i ARCHIVE, --archive ARCHIVE
-                                   Path to OMEX file which contains one or more SED-ML-
-                                   encoded simulation experiments
-             -o OUT_DIR, --out-dir OUT_DIR
-                                   Directory to save outputs
-             -v, --version         show program's version number and exit
-        
-        Usage through Docker container
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The entrypoint to the Docker image supports the same command-line
-        interface described above.
-        
-        For example, the following command could be used to use the Docker image
-        to execute the COMBINE/OMEX archive ``./modeling-study.omex`` and save
-        its outputs to ``./``.
-        
-        ::
-        
-           docker run \
-             --tty \
-             --rm \
-             --mount type=bind,source="$(pwd)",target=/root/in,readonly \
-             --mount type=bind,source="$(pwd)",target=/root/out \
-             ghcr.io/biosimulators/tellurium:latest \
-               -i /root/in/modeling-study.omex \
-               -o /root/out
-        
-        Documentation
-        -------------
-        
-        Documentation is available at
-        https://biosimulators.github.io/Biosimulators_tellurium/.
-        
-        License
-        -------
-        
-        This package is released under the `MIT license <LICENSE>`__.
-        
-        Development team
-        ----------------
-        
-        This package was developed by the `Center for Reproducible Biomedical
-        Modeling <http://reproduciblebiomodels.org>`__ and the `Karr
-        Lab <https://www.karrlab.org>`__ at the Icahn School of Medicine at
-        Mount Sinai in New York.
-        
-        Questions and comments
-        ----------------------
-        
-        Please contact the `BioSimulators
-        Team <mailto:info@biosimulators.org>`__ with any questions or comments.
-        
-        .. |Latest release| image:: https://img.shields.io/github/v/tag/biosimulators/Biosimulators_tellurium
-           :target: https://github.com/biosimulations/Biosimulators_tellurium/releases
-        .. |PyPI| image:: https://img.shields.io/pypi/v/biosimulators_tellurium
-           :target: https://pypi.org/project/biosimulators_tellurium/
-        .. |CI status| image:: https://github.com/biosimulators/Biosimulators_tellurium/workflows/Continuous%20integration/badge.svg
-           :target: https://github.com/biosimulators/Biosimulators_tellurium/actions?query=workflow%3A%22Continuous+integration%22
-        .. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_tellurium/branch/dev/graph/badge.svg
-           :target: https://codecov.io/gh/biosimulators/Biosimulators_tellurium
-        
 Keywords: systems biology,computational biology,kinetic modeling,numerical simulation,stochastic,SBML,SED-ML,COMBINE,BioSimulators
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: all
+License-File: LICENSE
+
+|Latest release| |PyPI| |CI status| |Test coverage|
+
+BioSimulators-tellurium
+=======================
+
+BioSimulators-compliant command-line interface and Docker image for the
+`tellurium <http://tellurium.analogmachine.org/>`__ simulation program.
+
+This command-line interface and Docker image enable users to use
+tellurium to execute `COMBINE/OMEX
+archives <https://combinearchive.org/>`__ that describe one or more
+simulation experiments (in `SED-ML format <https://sed-ml.org>`__) of
+one or more models (in `SBML format <http://sbml.org]>`__).
+
+A list of the algorithms and algorithm parameters supported by tellurium
+is available at
+`BioSimulators <https://biosimulators.org/simulators/tellurium>`__.
+
+A simple web application and web service for using tellurium to execute
+COMBINE/OMEX archives is also available at
+`runBioSimulations <https://run.biosimulations.org>`__.
+
+Installation
+------------
+
+Install Python package
+~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+   pip install biosimulators-tellurium
+
+Install Docker image
+~~~~~~~~~~~~~~~~~~~~
+
+::
+
+   docker pull ghcr.io/biosimulators/tellurium
+
+Usage
+-----
+
+Local usage
+~~~~~~~~~~~
+
+::
+
+   usage: tellurium [-h] [-d] [-q] -i ARCHIVE [-o OUT_DIR] [-v]
+
+   BioSimulators-compliant command-line interface to the tellurium simulation program <http://tellurium.analogmachine.org>.
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     -d, --debug           full application debug mode
+     -q, --quiet           suppress all console output
+     -i ARCHIVE, --archive ARCHIVE
+                           Path to OMEX file which contains one or more SED-ML-
+                           encoded simulation experiments
+     -o OUT_DIR, --out-dir OUT_DIR
+                           Directory to save outputs
+     -v, --version         show program's version number and exit
+
+Usage through Docker container
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The entrypoint to the Docker image supports the same command-line
+interface described above.
+
+For example, the following command could be used to use the Docker image
+to execute the COMBINE/OMEX archive ``./modeling-study.omex`` and save
+its outputs to ``./``.
+
+::
+
+   docker run \
+     --tty \
+     --rm \
+     --mount type=bind,source="$(pwd)",target=/root/in,readonly \
+     --mount type=bind,source="$(pwd)",target=/root/out \
+     ghcr.io/biosimulators/tellurium:latest \
+       -i /root/in/modeling-study.omex \
+       -o /root/out
+
+Documentation
+-------------
+
+Documentation is available at
+https://biosimulators.github.io/Biosimulators_tellurium/.
+
+License
+-------
+
+This package is released under the `MIT license <LICENSE>`__.
+
+Development team
+----------------
+
+This package was developed by the `Center for Reproducible Biomedical
+Modeling <http://reproduciblebiomodels.org>`__ and the `Karr
+Lab <https://www.karrlab.org>`__ at the Icahn School of Medicine at
+Mount Sinai in New York.
+
+Questions and comments
+----------------------
+
+Please contact the `BioSimulators
+Team <mailto:info@biosimulators.org>`__ with any questions or comments.
+
+.. |Latest release| image:: https://img.shields.io/github/v/tag/biosimulators/Biosimulators_tellurium
+   :target: https://github.com/biosimulations/Biosimulators_tellurium/releases
+.. |PyPI| image:: https://img.shields.io/pypi/v/biosimulators_tellurium
+   :target: https://pypi.org/project/biosimulators_tellurium/
+.. |CI status| image:: https://github.com/biosimulators/Biosimulators_tellurium/workflows/Continuous%20integration/badge.svg
+   :target: https://github.com/biosimulators/Biosimulators_tellurium/actions?query=workflow%3A%22Continuous+integration%22
+.. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_tellurium/branch/dev/graph/badge.svg
+   :target: https://codecov.io/gh/biosimulators/Biosimulators_tellurium
+
+
```

### Comparing `biosimulators_tellurium-0.1.8/biosimulators_tellurium.egg-info/SOURCES.txt` & `biosimulators_tellurium-0.1.9/biosimulators_tellurium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosimulators_tellurium-0.1.8/setup.py` & `biosimulators_tellurium-0.1.9/setup.py`

 * *Files identical despite different names*

