# Comparing `tmp/pdf_language_detector-0.0.8.tar.gz` & `tmp/pdf_language_detector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_language_detector-0.0.8.tar", max compression
+gzip compressed data, was "pdf_language_detector-0.0.9.tar", max compression
```

## Comparing `pdf_language_detector-0.0.8.tar` & `pdf_language_detector-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2772 2023-06-15 18:42:42.158079 pdf_language_detector-0.0.8/README.md
--rw-r--r--   0        0        0      744 2023-06-15 20:12:55.815424 pdf_language_detector-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.8/src/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-15 15:36:48.029796 pdf_language_detector-0.0.8/src/cli.py
--rw-r--r--   0        0        0    12932 2023-06-15 20:12:03.762975 pdf_language_detector-0.0.8/src/pld.py
--rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.8/src/report.py
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.8/setup.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3087 2023-06-16 08:55:09.790521 pdf_language_detector-0.0.9/README.md
+-rw-r--r--   0        0        0      908 2023-06-16 08:56:39.411240 pdf_language_detector-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-14 22:13:51.629533 pdf_language_detector-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     1649 2023-06-16 08:55:09.790521 pdf_language_detector-0.0.9/src/cli.py
+-rw-r--r--   0        0        0    13198 2023-06-16 08:55:09.790521 pdf_language_detector-0.0.9/src/pld.py
+-rw-r--r--   0        0        0     3735 2023-06-15 14:29:56.113761 pdf_language_detector-0.0.9/src/report.py
+-rw-r--r--   0        0        0     4229 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.9/setup.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 pdf_language_detector-0.0.9/PKG-INFO
```

### Comparing `pdf_language_detector-0.0.8/README.md` & `pdf_language_detector-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# PLD (PDF Language Detector)
+# PLD (PDF Language Detector)  [![](https://img.shields.io/github/actions/workflow/status/icij/pld/main.yml)](https://github.com/ICIJ/pld/actions)
+
 
 PLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.
 
 ## Requirements
 
 - [Python 3.8](https://www.python.org/downloads/) or above
 - [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
@@ -60,15 +61,14 @@
 
 Then run inside a container:
 
 ```bash
 docker run -it icij/pld pld --help
 ```
 
-
 ## Usage
 
 ### Detect
 
 This command process PDF files and detect the dominant language.
 
 ```
@@ -78,26 +78,35 @@
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
     --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
     --parallel (optional): Number of threads to run in parallel.
+    --relative-to (optional): Path to the directory relative to which build the output dir path.
 ```
 
 ### Report
 
 This command print a report from the previously detected language (using the same output dir).
 
 ```
 pld report --help
 
     --output-dir: Path to the output directory. Default is 'out' directory in the current directory.
 ```
 
+## Test
+
+You can run the test suite (propulsed by pytest) with this command:
+
+```bash
+make test
+```
+
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
 pld --language eng --language spa --input-dir documents --output-dir results
 ```
```

### Comparing `pdf_language_detector-0.0.8/src/cli.py` & `pdf_language_detector-0.0.9/src/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 def detect(languages: List[str] = typer.Option(..., '--language', help="An ISO3 language code."), 
          input_dir: Path  = typer.Option(..., '--input-dir', help="Path to the input directory."),
          output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory."),
          max_pages: Optional[int] = typer.Option(5, help="Maximum number of pages to process per PDF file."),
          resume: Optional[bool] = typer.Option(False, help="Skip PDF files already analyzed."),
          skip_images:  Optional[bool] = typer.Option(False, help="Skip the extraction of PDF files as images."),
          skip_ocr:  Optional[bool] = typer.Option(False, help="Skip the OCR of images from PDF files."),
-         parallel: Optional[int] = typer.Option(1, help="Number of paralell PDF to process in threads.")):
+         parallel: Optional[int] = typer.Option(1, help="Number of paralell PDF to process in threads."),
+         relative_to: Optional[Path] = typer.Option(None, help="Path to the directory relative to which build the output dir path.")):
     """
     Process PDF files and detect the dominant language.
     """
-    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, resume, skip_images, skip_ocr, parallel)
+    detector = PdfLanguageDetector(languages, input_dir, output_dir, max_pages, resume, 
+                                   skip_images, skip_ocr, parallel, relative_to)
     detector.process_input_files()
 
 @app.command()
 def report(output_dir: Optional[Path] = typer.Option('out', help="Path to the output directory.")):
     """
     Process generated files to output a report
     """
```

### Comparing `pdf_language_detector-0.0.8/src/pld.py` & `pdf_language_detector-0.0.9/src/pld.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,47 +11,50 @@
 from rich.progress import Progress, SpinnerColumn
 from sh import pdftoppm
 from typing import Optional, List
 
 class PdfLanguageDetector:
     STATUS_SKIPPED = 'SKIPPED'
     STATUS_DONE = 'DONE'
-    STATUS_FAILED = 'FAILED'
+    STATUS_FAILED = 'FAILED '
     
     def __init__(self, 
                 languages: List[str], 
                 input_dir: Path = Path(),
                 output_dir: Optional[Path] = 'out',
                 max_pages: Optional[int] = 5,
                 resume:  Optional[bool] = False,
                 skip_images:  Optional[bool] = False,
                 skip_ocr:  Optional[bool] = False,
-                parallel: Optional[int] = 1):
+                parallel: Optional[int] = 1,
+                relative_to: Optional[Path] = None):
         """
         Initialize the PdfLanguageDetector class.
 
         Args:
             languages: List of ISO3 language codes.
             input_dir: Path to the input directory.
             output_dir: Path to the output directory.
             max_pages: Maximum number of pages to process per PDF file.
             resume: Skip PDF files already analyzed.
             skip_images: Skip the extraction of PDF files as images.
             skip_ocr: Skip the OCR of images from PDF files.
             parallel: Number of threads to run in parallel.
+            relative_to: Path to the directory relative to which build the output dir path.
         """
         self.languages = [Language.get(language) for language in languages]
         self.lang_detector = LanguageDetectorBuilder.from_iso_codes_639_3(*self.lingua_langs).build()
         self.input_dir = input_dir
         self.output_dir = output_dir
         self.max_pages = max_pages
         self.resume = resume
         self.skip_images = skip_images
         self.skip_ocr = skip_ocr
         self.parallel = parallel
+        self.relative_to = input_dir.resolve() if relative_to is None else relative_to.resolve()
 
     def create_output_directories(self, *dirs: Path):
         """
         Create output directories if they don't exist.
 
         Args:
             *dirs: Variable number of directory paths to create.
@@ -97,15 +100,15 @@
         Args:
             image_text: Text to be saved.
             text_file: Path to the output text file.
         """
         with text_file.open("a") as f:
             f.write(image_text)
 
-    def save_language(self, detected_lang, lang_file: Path):
+    def save_language(self, detected_lang: List[list], lang_file: Path):
         """
         Save detected language information to a JSON file.
 
         Args:
             detected_lang: Language detection result.
             lang_file: Path to the output JSON file.
         """
@@ -293,15 +296,15 @@
 
         Args:
             input_file: Path to the input file.
 
         Returns:
             The output directory path.
         """
-        output_file_dir = input_file.relative_to(self.input_dir)
+        output_file_dir = input_file.resolve().relative_to(self.relative_to)
         output_file_dir = output_file_dir.parent / output_file_dir.stem
         output_file_dir = self.output_dir / output_file_dir
         return output_file_dir
     
     def is_already_analyzed(self, output_file_dir: Path) -> bool:
         return (output_file_dir / 'avgs.json').exists()
```

### Comparing `pdf_language_detector-0.0.8/src/report.py` & `pdf_language_detector-0.0.9/src/report.py`

 * *Files identical despite different names*

### Comparing `pdf_language_detector-0.0.8/setup.py` & `pdf_language_detector-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 entry_points = \
 {'console_scripts': ['pdf-language-detector = src.cli:app',
                      'pld = src.cli:app']}
 
 setup_kwargs = {
     'name': 'pdf-language-detector',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.',
-    'long_description': "# PLD (PDF Language Detector)\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n    --parallel (optional): Number of threads to run in parallel.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
+    'long_description': "# PLD (PDF Language Detector)  [![](https://img.shields.io/github/actions/workflow/status/icij/pld/main.yml)](https://github.com/ICIJ/pld/actions)\n\n\nPLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.\n\n## Requirements\n\n- [Python 3.8](https://www.python.org/downloads/) or above\n- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)\n- [pdftoppm](https://poppler.freedesktop.org/)\n\n## Installation\n\nInstall Tesseract OCR and pdftoppm using your package manager. For example, on Ubuntu:\n\n```bash\nsudo apt install tesseract-ocr tesseract-ocr-all poppler-utils\n```\n\n### From PyPi\n\nInstall with pip:\n\n```bash\npython3 -m pip install --user pdf-language-detector\n```\n\nThen run directly from your terminal:\n\n```bash\npld --help\n````\n\n### From the sources\n\nClone the PLD repository:\n\n```bash\ngit clone git@github.com:github.com/icij/pld.git\n```\n\nInstall the required Python packages with poetry:\n\n```bash\npoetry install\n````\n\nThen run inside a virtual env managed by poetry:\n\n```bash\npoetry run pld --help\n````\n\n### From Docker\n\nInstall with Docker:\n\n```bash\ndocker pull icij/pld\n```\n\nThen run inside a container:\n\n```bash\ndocker run -it icij/pld pld --help\n```\n\n## Usage\n\n### Detect\n\nThis command process PDF files and detect the dominant language.\n\n```\npld detect --help\n\n    --language A list of ISO3 language codes to detect.\n    --input-dir: Path to the input directory containing PDF files. Default is the current directory.\n    --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.\n    --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.\n    --resume (optional): Skip PDF files already analyzed.\n    --skip-images (optional): Skip the extraction of PDF files a images.\n    --skip-ocr (optional): Skip the OCR of images from PDF files.\n    --parallel (optional): Number of threads to run in parallel.\n    --relative-to (optional): Path to the directory relative to which build the output dir path.\n```\n\n### Report\n\nThis command print a report from the previously detected language (using the same output dir).\n\n```\npld report --help\n\n    --output-dir: Path to the output directory. Default is 'out' directory in the current directory.\n```\n\n## Test\n\nYou can run the test suite (propulsed by pytest) with this command:\n\n```bash\nmake test\n```\n\n## Examples\n\nProcess PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:\n\n```bash\npld --language eng --language spa --input-dir documents --output-dir results\n```\n\nProcess PDF files in the 'documents' directory, detect French and Greek languages, and limit the processing to 3 pages per file:\n\n```bash\npld --language fra --language ell --input-dir documents --max-pages 3\n```\n\n## License\n\nThis project is licensed under the MIT License.\n",
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pdf_language_detector-0.0.8/PKG-INFO` & `pdf_language_detector-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-language-detector
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python script to iterate over a list of PDF in a directory and try to guess their language with Tesseract OCR.
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,16 @@
 Requires-Dist: lingua-language-detector (>=1.3.2,<2.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: sh (>=2.0.4,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# PLD (PDF Language Detector)
+# PLD (PDF Language Detector)  [![](https://img.shields.io/github/actions/workflow/status/icij/pld/main.yml)](https://github.com/ICIJ/pld/actions)
+
 
 PLD is a Python program that analyzes PDF files, extracts images, processes them using Optical Character Recognition (OCR), and detects the dominant language of the text. It provides language detection information in JSON format and calculates the average confidence coefficient for each language.
 
 ## Requirements
 
 - [Python 3.8](https://www.python.org/downloads/) or above
 - [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
@@ -79,15 +80,14 @@
 
 Then run inside a container:
 
 ```bash
 docker run -it icij/pld pld --help
 ```
 
-
 ## Usage
 
 ### Detect
 
 This command process PDF files and detect the dominant language.
 
 ```
@@ -97,26 +97,35 @@
     --input-dir: Path to the input directory containing PDF files. Default is the current directory.
     --output-dir (optional): Path to the output directory. Default is 'out' directory in the current directory.
     --max-pages (optional): Maximum number of pages to process per PDF file. Default is 5.
     --resume (optional): Skip PDF files already analyzed.
     --skip-images (optional): Skip the extraction of PDF files a images.
     --skip-ocr (optional): Skip the OCR of images from PDF files.
     --parallel (optional): Number of threads to run in parallel.
+    --relative-to (optional): Path to the directory relative to which build the output dir path.
 ```
 
 ### Report
 
 This command print a report from the previously detected language (using the same output dir).
 
 ```
 pld report --help
 
     --output-dir: Path to the output directory. Default is 'out' directory in the current directory.
 ```
 
+## Test
+
+You can run the test suite (propulsed by pytest) with this command:
+
+```bash
+make test
+```
+
 ## Examples
 
 Process PDF files in the current directory, detect English and Spanish languages, and save the results in the 'results' directory:
 
 ```bash
 pld --language eng --language spa --input-dir documents --output-dir results
 ```
```

