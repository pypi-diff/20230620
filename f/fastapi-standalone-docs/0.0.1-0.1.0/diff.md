# Comparing `tmp/fastapi_standalone_docs-0.0.1.tar.gz` & `tmp/fastapi_standalone_docs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_standalone_docs-0.0.1.tar", max compression
+gzip compressed data, was "fastapi_standalone_docs-0.1.0.tar", max compression
```

## Comparing `fastapi_standalone_docs-0.0.1.tar` & `fastapi_standalone_docs-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/LICENSE
--rw-r--r--   0        0        0     4219 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/README.md
--rw-r--r--   0        0        0       82 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/__init__.py
--rw-r--r--   0        0        0     1826 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/scripts.py
--rw-r--r--   0        0        0     2709 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/standalone_docs.py
--rw-r--r--   0        0        0     1086 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/fastapi/LICENSE
--rw-r--r--   0        0        0      412 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/fastapi/favicon.png
--rw-r--r--   0        0        0     1174 2023-06-19 10:51:52.261341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/logo-mini.svg
--rw-r--r--   0        0        0  1042007 2023-06-19 10:51:52.269341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js
--rw-r--r--   0        0        0     2634 2023-06-19 10:51:52.269341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0    11358 2023-06-19 10:51:52.269341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/LICENSE
--rw-r--r--   0        0        0  1048219 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
--rw-r--r--   0        0        0   145206 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/swagger-ui.css
--rw-r--r--   0        0        0        0 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/tests/conftests.py
--rw-r--r--   0        0        0     5787 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/tests/test_standalone_docs.py
--rw-r--r--   0        0        0      785 2023-06-19 10:51:52.273341 fastapi_standalone_docs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4618 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/README.md
+-rw-r--r--   0        0        0       82 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/__init__.py
+-rw-r--r--   0        0        0     1828 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/scripts.py
+-rw-r--r--   0        0        0     2759 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/standalone_docs.py
+-rw-r--r--   0        0        0     1086 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/fastapi/LICENSE
+-rw-r--r--   0        0        0      412 2023-06-20 09:54:52.594960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/fastapi/favicon.png
+-rw-r--r--   0        0        0     1174 2023-06-20 09:54:52.598960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/logo-mini.svg
+-rw-r--r--   0        0        0  1042510 2023-06-20 09:54:52.602960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/redoc.standalone.js
+-rw-r--r--   0        0        0     2628 2023-06-20 09:54:52.602960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0    11358 2023-06-20 09:54:52.602960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/LICENSE
+-rw-r--r--   0        0        0  1048219 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   145206 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/swagger-ui.css
+-rw-r--r--   0        0        0        0 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/tests/conftests.py
+-rw-r--r--   0        0        0     6131 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/tests/test_standalone_docs.py
+-rw-r--r--   0        0        0      785 2023-06-20 09:54:52.610960 fastapi_standalone_docs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.0/PKG-INFO
```

### Comparing `fastapi_standalone_docs-0.0.1/LICENSE` & `fastapi_standalone_docs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/README.md` & `fastapi_standalone_docs-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,22 @@
 app = FastAPI()
 StandaloneDocs(
     app=app,
     with_google_fonts=True,
 )
 ```
 
+### Disclaimer
+
+**Note!** If you create multiple FastAPI apps in the same runtime (quite unlikely
+use-case), using StandaloneDocs on one of them will affect the other ones as well, as
+the library patches two of the shared functions (`get_swagger_ui_html` and
+`get_redoc_html`). Thus the library should not be used in a such setup unless all the
+apps will use StandaloneDocs with the same settings.
+
 ## Development
 
 PRs are welcome!
 
 This project is using [Poetry](https://python-poetry.org/) and
 [pre-commit](https://pre-commit.com/), so please ensure you've installed both. To set up
 the project with them run:
```

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/scripts.py` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/scripts.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 SWAGGER_FILES = [
     "https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/LICENSE",
     "https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui.css",
     "https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui-bundle.js",
 ]
 
 REDOC_FILES = [
-    "https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js.LICENSE.txt",
-    "https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js",
+    "https://cdn.jsdelivr.net/npm/redoc@2.0.0/bundles/redoc.standalone.js.LICENSE.txt",
+    "https://cdn.jsdelivr.net/npm/redoc@2.0.0/bundles/redoc.standalone.js",
     "https://cdn.redoc.ly/redoc/logo-mini.svg",
 ]
 
 
 def update_docs():
     static_path = Path(fastapi_standalone_docs.__path__[0]) / "static"
     fastapi_path = static_path / "fastapi"
```

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/standalone_docs.py` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/standalone_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.with_google_fonts = with_google_fonts
         self.static_path = Path(fastapi_standalone_docs.__path__[0]) / "static"
 
         self.patch_swagger(swagger_favicon_url)
         self.patch_redoc(redoc_favicon_url)
 
     def patch_swagger(self, swagger_favicon_url: Optional[str]):
-        if self.app.docs_url:
+        if self.app.openapi_url and self.app.docs_url:
             if not swagger_favicon_url:
                 swagger_favicon_url = self.app.docs_url + "/fastapi/favicon.png"
                 self.app.mount(
                     self.app.docs_url + "/fastapi/",
                     StaticFiles(directory=self.static_path / "fastapi"),
                 )
 
@@ -45,15 +45,15 @@
                     swagger_css_url=self.app.docs_url + "/swagger-ui.css",
                     swagger_js_url=self.app.docs_url + "/swagger-ui-bundle.js",
                 )
 
             applications.get_swagger_ui_html = patched_get_swagger_ui_html
 
     def patch_redoc(self, redoc_favicon_url: Optional[str]):
-        if self.app.redoc_url:
+        if self.app.openapi_url and self.app.redoc_url:
             if not redoc_favicon_url:
                 redoc_favicon_url = self.app.redoc_url + "/fastapi/favicon.png"
                 self.app.mount(
                     self.app.redoc_url + "/fastapi/",
                     StaticFiles(directory=self.static_path / "fastapi"),
                 )
```

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/fastapi/LICENSE` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/fastapi/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/logo-mini.svg` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/logo-mini.svg`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/redoc.standalone.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27516,15 +27516,15 @@
                                 }, new e
                             }()
                         },
                         6980: function(e, t, n) {
                             var r = n(6314),
                                 o = ["add", "done", "toJS", "fromExternalJS", "load", "dispose", "search", "Worker"];
                             e.exports = function() {
-                                var e = new Worker(URL.createObjectURL(new Blob(['/*! For license information please see 9e68c24da9f5fd56991c.worker.js.LICENSE.txt */\n!function(){var e={336:function(e,t,r){var n,i;!function(){var s,o,a,u,l,c,h,d,f,p,y,m,g,x,v,w,Q,k,S,E,L,P,b,T,O,I,R=function(e){var t=new R.Builder;return t.pipeline.add(R.trimmer,R.stopWordFilter,R.stemmer),t.searchPipeline.add(R.stemmer),e.call(t,t),t.build()};R.version="2.3.9",R.utils={},R.utils.warn=(s=this,function(e){s.console&&console.warn&&console.warn(e)}),R.utils.asString=function(e){return null==e?"":e.toString()},R.utils.clone=function(e){if(null==e)return e;for(var t=Object.create(null),r=Object.keys(e),n=0;n<r.length;n++){var i=r[n],s=e[i];if(Array.isArray(s))t[i]=s.slice();else{if("string"!=typeof s&&"number"!=typeof s&&"boolean"!=typeof s)throw new TypeError("clone is not deep and does not support nested objects");t[i]=s}}return t},R.FieldRef=function(e,t,r){this.docRef=e,this.fieldName=t,this._stringValue=r},R.FieldRef.joiner="/",R.FieldRef.fromString=function(e){var t=e.indexOf(R.FieldRef.joiner);if(-1===t)throw"malformed field ref string";var r=e.slice(0,t),n=e.slice(t+1);return new R.FieldRef(n,r,e)},R.FieldRef.prototype.toString=function(){return null==this._stringValue&&(this._stringValue=this.fieldName+R.FieldRef.joiner+this.docRef),this._stringValue},R.Set=function(e){if(this.elements=Object.create(null),e){this.length=e.length;for(var t=0;t<this.length;t++)this.elements[e[t]]=!0}else this.length=0},R.Set.complete={intersect:function(e){return e},union:function(){return this},contains:function(){return!0}},R.Set.empty={intersect:function(){return this},union:function(e){return e},contains:function(){return!1}},R.Set.prototype.contains=function(e){return!!this.elements[e]},R.Set.prototype.intersect=function(e){var t,r,n,i=[];if(e===R.Set.complete)return this;if(e===R.Set.empty)return e;this.length<e.length?(t=this,r=e):(t=e,r=this),n=Object.keys(t.elements);for(var s=0;s<n.length;s++){var o=n[s];o in r.elements&&i.push(o)}return new R.Set(i)},R.Set.prototype.union=function(e){return e===R.Set.complete?R.Set.complete:e===R.Set.empty?this:new R.Set(Object.keys(this.elements).concat(Object.keys(e.elements)))},R.idf=function(e,t){var r=0;for(var n in e)"_index"!=n&&(r+=Object.keys(e[n]).length);var i=(t-r+.5)/(r+.5);return Math.log(1+Math.abs(i))},R.Token=function(e,t){this.str=e||"",this.metadata=t||{}},R.Token.prototype.toString=function(){return this.str},R.Token.prototype.update=function(e){return this.str=e(this.str,this.metadata),this},R.Token.prototype.clone=function(e){return e=e||function(e){return e},new R.Token(e(this.str,this.metadata),this.metadata)},R.tokenizer=function(e,t){if(null==e||null==e)return[];if(Array.isArray(e))return e.map((function(e){return new R.Token(R.utils.asString(e).toLowerCase(),R.utils.clone(t))}));for(var r=e.toString().toLowerCase(),n=r.length,i=[],s=0,o=0;s<=n;s++){var a=s-o;if(r.charAt(s).match(R.tokenizer.separator)||s==n){if(a>0){var u=R.utils.clone(t)||{};u.position=[o,a],u.index=i.length,i.push(new R.Token(r.slice(o,s),u))}o=s+1}}return i},R.tokenizer.separator=/[\\s\\-]+/,R.Pipeline=function(){this._stack=[]},R.Pipeline.registeredFunctions=Object.create(null),R.Pipeline.registerFunction=function(e,t){t in this.registeredFunctions&&R.utils.warn("Overwriting existing registered function: "+t),e.label=t,R.Pipeline.registeredFunctions[e.label]=e},R.Pipeline.warnIfFunctionNotRegistered=function(e){e.label&&e.label in this.registeredFunctions||R.utils.warn("Function is not registered with pipeline. This may cause problems when serialising the index.\\n",e)},R.Pipeline.load=function(e){var t=new R.Pipeline;return e.forEach((function(e){var r=R.Pipeline.registeredFunctions[e];if(!r)throw new Error("Cannot load unregistered function: "+e);t.add(r)})),t},R.Pipeline.prototype.add=function(){var e=Array.prototype.slice.call(arguments);e.forEach((function(e){R.Pipeline.warnIfFunctionNotRegistered(e),this._stack.push(e)}),this)},R.Pipeline.prototype.after=function(e,t){R.Pipeline.warnIfFunctionNotRegistered(t);var r=this._stack.indexOf(e);if(-1==r)throw new Error("Cannot find existingFn");r+=1,this._stack.splice(r,0,t)},R.Pipeline.prototype.before=function(e,t){R.Pipeline.warnIfFunctionNotRegistered(t);var r=this._stack.indexOf(e);if(-1==r)throw new Error("Cannot find existingFn");this._stack.splice(r,0,t)},R.Pipeline.prototype.remove=function(e){var t=this._stack.indexOf(e);-1!=t&&this._stack.splice(t,1)},R.Pipeline.prototype.run=function(e){for(var t=this._stack.length,r=0;r<t;r++){for(var n=this._stack[r],i=[],s=0;s<e.length;s++){var o=n(e[s],s,e);if(null!=o&&""!==o)if(Array.isArray(o))for(var a=0;a<o.length;a++)i.push(o[a]);else i.push(o)}e=i}return e},R.Pipeline.prototype.runString=function(e,t){var r=new R.Token(e,t);return this.run([r]).map((function(e){return e.toString()}))},R.Pipeline.prototype.reset=function(){this._stack=[]},R.Pipeline.prototype.toJSON=function(){return this._stack.map((function(e){return R.Pipeline.warnIfFunctionNotRegistered(e),e.label}))},R.Vector=function(e){this._magnitude=0,this.elements=e||[]},R.Vector.prototype.positionForIndex=function(e){if(0==this.elements.length)return 0;for(var t=0,r=this.elements.length/2,n=r-t,i=Math.floor(n/2),s=this.elements[2*i];n>1&&(s<e&&(t=i),s>e&&(r=i),s!=e);)n=r-t,i=t+Math.floor(n/2),s=this.elements[2*i];return s==e||s>e?2*i:s<e?2*(i+1):void 0},R.Vector.prototype.insert=function(e,t){this.upsert(e,t,(function(){throw"duplicate index"}))},R.Vector.prototype.upsert=function(e,t,r){this._magnitude=0;var n=this.positionForIndex(e);this.elements[n]==e?this.elements[n+1]=r(this.elements[n+1],t):this.elements.splice(n,0,e,t)},R.Vector.prototype.magnitude=function(){if(this._magnitude)return this._magnitude;for(var e=0,t=this.elements.length,r=1;r<t;r+=2){var n=this.elements[r];e+=n*n}return this._magnitude=Math.sqrt(e)},R.Vector.prototype.dot=function(e){for(var t=0,r=this.elements,n=e.elements,i=r.length,s=n.length,o=0,a=0,u=0,l=0;u<i&&l<s;)(o=r[u])<(a=n[l])?u+=2:o>a?l+=2:o==a&&(t+=r[u+1]*n[l+1],u+=2,l+=2);return t},R.Vector.prototype.similarity=function(e){return this.dot(e)/this.magnitude()||0},R.Vector.prototype.toArray=function(){for(var e=new Array(this.elements.length/2),t=1,r=0;t<this.elements.length;t+=2,r++)e[r]=this.elements[t];return e},R.Vector.prototype.toJSON=function(){return this.elements},R.stemmer=(o={ational:"ate",tional:"tion",enci:"ence",anci:"ance",izer:"ize",bli:"ble",alli:"al",entli:"ent",eli:"e",ousli:"ous",ization:"ize",ation:"ate",ator:"ate",alism:"al",iveness:"ive",fulness:"ful",ousness:"ous",aliti:"al",iviti:"ive",biliti:"ble",logi:"log"},a={icate:"ic",ative:"",alize:"al",iciti:"ic",ical:"ic",ful:"",ness:""},u="[aeiouy]",l="[^aeiou][^aeiouy]*",c=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*"),h=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*[aeiouy][aeiou]*[^aeiou][^aeiouy]*"),d=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*([aeiouy][aeiou]*)?$"),f=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy]"),p=/^(.+?)(ss|i)es$/,y=/^(.+?)([^s])s$/,m=/^(.+?)eed$/,g=/^(.+?)(ed|ing)$/,x=/.$/,v=/(at|bl|iz)$/,w=new RegExp("([^aeiouylsz])\\\\1$"),Q=new RegExp("^"+l+u+"[^aeiouwxy]$"),k=/^(.+?[^aeiou])y$/,S=/^(.+?)(ational|tional|enci|anci|izer|bli|alli|entli|eli|ousli|ization|ation|ator|alism|iveness|fulness|ousness|aliti|iviti|biliti|logi)$/,E=/^(.+?)(icate|ative|alize|iciti|ical|ful|ness)$/,L=/^(.+?)(al|ance|ence|er|ic|able|ible|ant|ement|ment|ent|ou|ism|ate|iti|ous|ive|ize)$/,P=/^(.+?)(s|t)(ion)$/,b=/^(.+?)e$/,T=/ll$/,O=new RegExp("^"+l+u+"[^aeiouwxy]$"),I=function(e){var t,r,n,i,s,u,l;if(e.length<3)return e;if("y"==(n=e.substr(0,1))&&(e=n.toUpperCase()+e.substr(1)),s=y,(i=p).test(e)?e=e.replace(i,"$1$2"):s.test(e)&&(e=e.replace(s,"$1$2")),s=g,(i=m).test(e)){var I=i.exec(e);(i=c).test(I[1])&&(i=x,e=e.replace(i,""))}else s.test(e)&&(t=(I=s.exec(e))[1],(s=f).test(t)&&(u=w,l=Q,(s=v).test(e=t)?e+="e":u.test(e)?(i=x,e=e.replace(i,"")):l.test(e)&&(e+="e")));return(i=k).test(e)&&(e=(t=(I=i.exec(e))[1])+"i"),(i=S).test(e)&&(t=(I=i.exec(e))[1],r=I[2],(i=c).test(t)&&(e=t+o[r])),(i=E).test(e)&&(t=(I=i.exec(e))[1],r=I[2],(i=c).test(t)&&(e=t+a[r])),s=P,(i=L).test(e)?(t=(I=i.exec(e))[1],(i=h).test(t)&&(e=t)):s.test(e)&&(t=(I=s.exec(e))[1]+I[2],(s=h).test(t)&&(e=t)),(i=b).test(e)&&(t=(I=i.exec(e))[1],s=d,u=O,((i=h).test(t)||s.test(t)&&!u.test(t))&&(e=t)),s=h,(i=T).test(e)&&s.test(e)&&(i=x,e=e.replace(i,"")),"y"==n&&(e=n.toLowerCase()+e.substr(1)),e},function(e){return e.update(I)}),R.Pipeline.registerFunction(R.stemmer,"stemmer"),R.generateStopWordFilter=function(e){var t=e.reduce((function(e,t){return e[t]=t,e}),{});return function(e){if(e&&t[e.toString()]!==e.toString())return e}},R.stopWordFilter=R.generateStopWordFilter(["a","able","about","across","after","all","almost","also","am","among","an","and","any","are","as","at","be","because","been","but","by","can","cannot","could","dear","did","do","does","either","else","ever","every","for","from","get","got","had","has","have","he","her","hers","him","his","how","however","i","if","in","into","is","it","its","just","least","let","like","likely","may","me","might","most","must","my","neither","no","nor","not","of","off","often","on","only","or","other","our","own","rather","said","say","says","she","should","since","so","some","than","that","the","their","them","then","there","these","they","this","tis","to","too","twas","us","wants","was","we","were","what","when","where","which","while","who","whom","why","will","with","would","yet","you","your"]),R.Pipeline.registerFunction(R.stopWordFilter,"stopWordFilter"),R.trimmer=function(e){return e.update((function(e){return e.replace(/^\\W+/,"").replace(/\\W+$/,"")}))},R.Pipeline.registerFunction(R.trimmer,"trimmer"),R.TokenSet=function(){this.final=!1,this.edges={},this.id=R.TokenSet._nextId,R.TokenSet._nextId+=1},R.TokenSet._nextId=1,R.TokenSet.fromArray=function(e){for(var t=new R.TokenSet.Builder,r=0,n=e.length;r<n;r++)t.insert(e[r]);return t.finish(),t.root},R.TokenSet.fromClause=function(e){return"editDistance"in e?R.TokenSet.fromFuzzyString(e.term,e.editDistance):R.TokenSet.fromString(e.term)},R.TokenSet.fromFuzzyString=function(e,t){for(var r=new R.TokenSet,n=[{node:r,editsRemaining:t,str:e}];n.length;){var i=n.pop();if(i.str.length>0){var s,o=i.str.charAt(0);o in i.node.edges?s=i.node.edges[o]:(s=new R.TokenSet,i.node.edges[o]=s),1==i.str.length&&(s.final=!0),n.push({node:s,editsRemaining:i.editsRemaining,str:i.str.slice(1)})}if(0!=i.editsRemaining){if("*"in i.node.edges)var a=i.node.edges["*"];else a=new R.TokenSet,i.node.edges["*"]=a;if(0==i.str.length&&(a.final=!0),n.push({node:a,editsRemaining:i.editsRemaining-1,str:i.str}),i.str.length>1&&n.push({node:i.node,editsRemaining:i.editsRemaining-1,str:i.str.slice(1)}),1==i.str.length&&(i.node.final=!0),i.str.length>=1){if("*"in i.node.edges)var u=i.node.edges["*"];else u=new R.TokenSet,i.node.edges["*"]=u;1==i.str.length&&(u.final=!0),n.push({node:u,editsRemaining:i.editsRemaining-1,str:i.str.slice(1)})}if(i.str.length>1){var l,c=i.str.charAt(0),h=i.str.charAt(1);h in i.node.edges?l=i.node.edges[h]:(l=new R.TokenSet,i.node.edges[h]=l),1==i.str.length&&(l.final=!0),n.push({node:l,editsRemaining:i.editsRemaining-1,str:c+i.str.slice(2)})}}}return r},R.TokenSet.fromString=function(e){for(var t=new R.TokenSet,r=t,n=0,i=e.length;n<i;n++){var s=e[n],o=n==i-1;if("*"==s)t.edges[s]=t,t.final=o;else{var a=new R.TokenSet;a.final=o,t.edges[s]=a,t=a}}return r},R.TokenSet.prototype.toArray=function(){for(var e=[],t=[{prefix:"",node:this}];t.length;){var r=t.pop(),n=Object.keys(r.node.edges),i=n.length;r.node.final&&(r.prefix.charAt(0),e.push(r.prefix));for(var s=0;s<i;s++){var o=n[s];t.push({prefix:r.prefix.concat(o),node:r.node.edges[o]})}}return e},R.TokenSet.prototype.toString=function(){if(this._str)return this._str;for(var e=this.final?"1":"0",t=Object.keys(this.edges).sort(),r=t.length,n=0;n<r;n++){var i=t[n];e=e+i+this.edges[i].id}return e},R.TokenSet.prototype.intersect=function(e){for(var t=new R.TokenSet,r=void 0,n=[{qNode:e,output:t,node:this}];n.length;){r=n.pop();for(var i=Object.keys(r.qNode.edges),s=i.length,o=Object.keys(r.node.edges),a=o.length,u=0;u<s;u++)for(var l=i[u],c=0;c<a;c++){var h=o[c];if(h==l||"*"==l){var d=r.node.edges[h],f=r.qNode.edges[l],p=d.final&&f.final,y=void 0;h in r.output.edges?(y=r.output.edges[h]).final=y.final||p:((y=new R.TokenSet).final=p,r.output.edges[h]=y),n.push({qNode:f,output:y,node:d})}}}return t},R.TokenSet.Builder=function(){this.previousWord="",this.root=new R.TokenSet,this.uncheckedNodes=[],this.minimizedNodes={}},R.TokenSet.Builder.prototype.insert=function(e){var t,r=0;if(e<this.previousWord)throw new Error("Out of order word insertion");for(var n=0;n<e.length&&n<this.previousWord.length&&e[n]==this.previousWord[n];n++)r++;for(this.minimize(r),t=0==this.uncheckedNodes.length?this.root:this.uncheckedNodes[this.uncheckedNodes.length-1].child,n=r;n<e.length;n++){var i=new R.TokenSet,s=e[n];t.edges[s]=i,this.uncheckedNodes.push({parent:t,char:s,child:i}),t=i}t.final=!0,this.previousWord=e},R.TokenSet.Builder.prototype.finish=function(){this.minimize(0)},R.TokenSet.Builder.prototype.minimize=function(e){for(var t=this.uncheckedNodes.length-1;t>=e;t--){var r=this.uncheckedNodes[t],n=r.child.toString();n in this.minimizedNodes?r.parent.edges[r.char]=this.minimizedNodes[n]:(r.child._str=n,this.minimizedNodes[n]=r.child),this.uncheckedNodes.pop()}},R.Index=function(e){this.invertedIndex=e.invertedIndex,this.fieldVectors=e.fieldVectors,this.tokenSet=e.tokenSet,this.fields=e.fields,this.pipeline=e.pipeline},R.Index.prototype.search=function(e){return this.query((function(t){new R.QueryParser(e,t).parse()}))},R.Index.prototype.query=function(e){for(var t=new R.Query(this.fields),r=Object.create(null),n=Object.create(null),i=Object.create(null),s=Object.create(null),o=Object.create(null),a=0;a<this.fields.length;a++)n[this.fields[a]]=new R.Vector;for(e.call(t,t),a=0;a<t.clauses.length;a++){var u,l=t.clauses[a],c=R.Set.empty;u=l.usePipeline?this.pipeline.runString(l.term,{fields:l.fields}):[l.term];for(var h=0;h<u.length;h++){var d=u[h];l.term=d;var f=R.TokenSet.fromClause(l),p=this.tokenSet.intersect(f).toArray();if(0===p.length&&l.presence===R.Query.presence.REQUIRED){for(var y=0;y<l.fields.length;y++)s[F=l.fields[y]]=R.Set.empty;break}for(var m=0;m<p.length;m++){var g=p[m],x=this.invertedIndex[g],v=x._index;for(y=0;y<l.fields.length;y++){var w=x[F=l.fields[y]],Q=Object.keys(w),k=g+"/"+F,S=new R.Set(Q);if(l.presence==R.Query.presence.REQUIRED&&(c=c.union(S),void 0===s[F]&&(s[F]=R.Set.complete)),l.presence!=R.Query.presence.PROHIBITED){if(n[F].upsert(v,l.boost,(function(e,t){return e+t})),!i[k]){for(var E=0;E<Q.length;E++){var L,P=Q[E],b=new R.FieldRef(P,F),T=w[P];void 0===(L=r[b])?r[b]=new R.MatchData(g,F,T):L.add(g,F,T)}i[k]=!0}}else void 0===o[F]&&(o[F]=R.Set.empty),o[F]=o[F].union(S)}}}if(l.presence===R.Query.presence.REQUIRED)for(y=0;y<l.fields.length;y++)s[F=l.fields[y]]=s[F].intersect(c)}var O=R.Set.complete,I=R.Set.empty;for(a=0;a<this.fields.length;a++){var F;s[F=this.fields[a]]&&(O=O.intersect(s[F])),o[F]&&(I=I.union(o[F]))}var C=Object.keys(r),N=[],j=Object.create(null);if(t.isNegated())for(C=Object.keys(this.fieldVectors),a=0;a<C.length;a++){b=C[a];var _=R.FieldRef.fromString(b);r[b]=new R.MatchData}for(a=0;a<C.length;a++){var D=(_=R.FieldRef.fromString(C[a])).docRef;if(O.contains(D)&&!I.contains(D)){var A,B=this.fieldVectors[_],z=n[_.fieldName].similarity(B);if(void 0!==(A=j[D]))A.score+=z,A.matchData.combine(r[_]);else{var V={ref:D,score:z,matchData:r[_]};j[D]=V,N.push(V)}}}return N.sort((function(e,t){return t.score-e.score}))},R.Index.prototype.toJSON=function(){var e=Object.keys(this.invertedIndex).sort().map((function(e){return[e,this.invertedIndex[e]]}),this),t=Object.keys(this.fieldVectors).map((function(e){return[e,this.fieldVectors[e].toJSON()]}),this);return{version:R.version,fields:this.fields,fieldVectors:t,invertedIndex:e,pipeline:this.pipeline.toJSON()}},R.Index.load=function(e){var t={},r={},n=e.fieldVectors,i=Object.create(null),s=e.invertedIndex,o=new R.TokenSet.Builder,a=R.Pipeline.load(e.pipeline);e.version!=R.version&&R.utils.warn("Version mismatch when loading serialised index. Current version of lunr \'"+R.version+"\' does not match serialized index \'"+e.version+"\'");for(var u=0;u<n.length;u++){var l=(h=n[u])[0],c=h[1];r[l]=new R.Vector(c)}for(u=0;u<s.length;u++){var h,d=(h=s[u])[0],f=h[1];o.insert(d),i[d]=f}return o.finish(),t.fields=e.fields,t.fieldVectors=r,t.invertedIndex=i,t.tokenSet=o.root,t.pipeline=a,new R.Index(t)},R.Builder=function(){this._ref="id",this._fields=Object.create(null),this._documents=Object.create(null),this.invertedIndex=Object.create(null),this.fieldTermFrequencies={},this.fieldLengths={},this.tokenizer=R.tokenizer,this.pipeline=new R.Pipeline,this.searchPipeline=new R.Pipeline,this.documentCount=0,this._b=.75,this._k1=1.2,this.termIndex=0,this.metadataWhitelist=[]},R.Builder.prototype.ref=function(e){this._ref=e},R.Builder.prototype.field=function(e,t){if(/\\//.test(e))throw new RangeError("Field \'"+e+"\' contains illegal character \'/\'");this._fields[e]=t||{}},R.Builder.prototype.b=function(e){this._b=e<0?0:e>1?1:e},R.Builder.prototype.k1=function(e){this._k1=e},R.Builder.prototype.add=function(e,t){var r=e[this._ref],n=Object.keys(this._fields);this._documents[r]=t||{},this.documentCount+=1;for(var i=0;i<n.length;i++){var s=n[i],o=this._fields[s].extractor,a=o?o(e):e[s],u=this.tokenizer(a,{fields:[s]}),l=this.pipeline.run(u),c=new R.FieldRef(r,s),h=Object.create(null);this.fieldTermFrequencies[c]=h,this.fieldLengths[c]=0,this.fieldLengths[c]+=l.length;for(var d=0;d<l.length;d++){var f=l[d];if(null==h[f]&&(h[f]=0),h[f]+=1,null==this.invertedIndex[f]){var p=Object.create(null);p._index=this.termIndex,this.termIndex+=1;for(var y=0;y<n.length;y++)p[n[y]]=Object.create(null);this.invertedIndex[f]=p}null==this.invertedIndex[f][s][r]&&(this.invertedIndex[f][s][r]=Object.create(null));for(var m=0;m<this.metadataWhitelist.length;m++){var g=this.metadataWhitelist[m],x=f.metadata[g];null==this.invertedIndex[f][s][r][g]&&(this.invertedIndex[f][s][r][g]=[]),this.invertedIndex[f][s][r][g].push(x)}}}},R.Builder.prototype.calculateAverageFieldLengths=function(){for(var e=Object.keys(this.fieldLengths),t=e.length,r={},n={},i=0;i<t;i++){var s=R.FieldRef.fromString(e[i]),o=s.fieldName;n[o]||(n[o]=0),n[o]+=1,r[o]||(r[o]=0),r[o]+=this.fieldLengths[s]}var a=Object.keys(this._fields);for(i=0;i<a.length;i++){var u=a[i];r[u]=r[u]/n[u]}this.averageFieldLength=r},R.Builder.prototype.createFieldVectors=function(){for(var e={},t=Object.keys(this.fieldTermFrequencies),r=t.length,n=Object.create(null),i=0;i<r;i++){for(var s=R.FieldRef.fromString(t[i]),o=s.fieldName,a=this.fieldLengths[s],u=new R.Vector,l=this.fieldTermFrequencies[s],c=Object.keys(l),h=c.length,d=this._fields[o].boost||1,f=this._documents[s.docRef].boost||1,p=0;p<h;p++){var y,m,g,x=c[p],v=l[x],w=this.invertedIndex[x]._index;void 0===n[x]?(y=R.idf(this.invertedIndex[x],this.documentCount),n[x]=y):y=n[x],m=y*((this._k1+1)*v)/(this._k1*(1-this._b+this._b*(a/this.averageFieldLength[o]))+v),m*=d,m*=f,g=Math.round(1e3*m)/1e3,u.insert(w,g)}e[s]=u}this.fieldVectors=e},R.Builder.prototype.createTokenSet=function(){this.tokenSet=R.TokenSet.fromArray(Object.keys(this.invertedIndex).sort())},R.Builder.prototype.build=function(){return this.calculateAverageFieldLengths(),this.createFieldVectors(),this.createTokenSet(),new R.Index({invertedIndex:this.invertedIndex,fieldVectors:this.fieldVectors,tokenSet:this.tokenSet,fields:Object.keys(this._fields),pipeline:this.searchPipeline})},R.Builder.prototype.use=function(e){var t=Array.prototype.slice.call(arguments,1);t.unshift(this),e.apply(this,t)},R.MatchData=function(e,t,r){for(var n=Object.create(null),i=Object.keys(r||{}),s=0;s<i.length;s++){var o=i[s];n[o]=r[o].slice()}this.metadata=Object.create(null),void 0!==e&&(this.metadata[e]=Object.create(null),this.metadata[e][t]=n)},R.MatchData.prototype.combine=function(e){for(var t=Object.keys(e.metadata),r=0;r<t.length;r++){var n=t[r],i=Object.keys(e.metadata[n]);null==this.metadata[n]&&(this.metadata[n]=Object.create(null));for(var s=0;s<i.length;s++){var o=i[s],a=Object.keys(e.metadata[n][o]);null==this.metadata[n][o]&&(this.metadata[n][o]=Object.create(null));for(var u=0;u<a.length;u++){var l=a[u];null==this.metadata[n][o][l]?this.metadata[n][o][l]=e.metadata[n][o][l]:this.metadata[n][o][l]=this.metadata[n][o][l].concat(e.metadata[n][o][l])}}}},R.MatchData.prototype.add=function(e,t,r){if(!(e in this.metadata))return this.metadata[e]=Object.create(null),void(this.metadata[e][t]=r);if(t in this.metadata[e])for(var n=Object.keys(r),i=0;i<n.length;i++){var s=n[i];s in this.metadata[e][t]?this.metadata[e][t][s]=this.metadata[e][t][s].concat(r[s]):this.metadata[e][t][s]=r[s]}else this.metadata[e][t]=r},R.Query=function(e){this.clauses=[],this.allFields=e},R.Query.wildcard=new String("*"),R.Query.wildcard.NONE=0,R.Query.wildcard.LEADING=1,R.Query.wildcard.TRAILING=2,R.Query.presence={OPTIONAL:1,REQUIRED:2,PROHIBITED:3},R.Query.prototype.clause=function(e){return"fields"in e||(e.fields=this.allFields),"boost"in e||(e.boost=1),"usePipeline"in e||(e.usePipeline=!0),"wildcard"in e||(e.wildcard=R.Query.wildcard.NONE),e.wildcard&R.Query.wildcard.LEADING&&e.term.charAt(0)!=R.Query.wildcard&&(e.term="*"+e.term),e.wildcard&R.Query.wildcard.TRAILING&&e.term.slice(-1)!=R.Query.wildcard&&(e.term=e.term+"*"),"presence"in e||(e.presence=R.Query.presence.OPTIONAL),this.clauses.push(e),this},R.Query.prototype.isNegated=function(){for(var e=0;e<this.clauses.length;e++)if(this.clauses[e].presence!=R.Query.presence.PROHIBITED)return!1;return!0},R.Query.prototype.term=function(e,t){if(Array.isArray(e))return e.forEach((function(e){this.term(e,R.utils.clone(t))}),this),this;var r=t||{};return r.term=e.toString(),this.clause(r),this},R.QueryParseError=function(e,t,r){this.name="QueryParseError",this.message=e,this.start=t,this.end=r},R.QueryParseError.prototype=new Error,R.QueryLexer=function(e){this.lexemes=[],this.str=e,this.length=e.length,this.pos=0,this.start=0,this.escapeCharPositions=[]},R.QueryLexer.prototype.run=function(){for(var e=R.QueryLexer.lexText;e;)e=e(this)},R.QueryLexer.prototype.sliceString=function(){for(var e=[],t=this.start,r=this.pos,n=0;n<this.escapeCharPositions.length;n++)r=this.escapeCharPositions[n],e.push(this.str.slice(t,r)),t=r+1;return e.push(this.str.slice(t,this.pos)),this.escapeCharPositions.length=0,e.join("")},R.QueryLexer.prototype.emit=function(e){this.lexemes.push({type:e,str:this.sliceString(),start:this.start,end:this.pos}),this.start=this.pos},R.QueryLexer.prototype.escapeCharacter=function(){this.escapeCharPositions.push(this.pos-1),this.pos+=1},R.QueryLexer.prototype.next=function(){if(this.pos>=this.length)return R.QueryLexer.EOS;var e=this.str.charAt(this.pos);return this.pos+=1,e},R.QueryLexer.prototype.width=function(){return this.pos-this.start},R.QueryLexer.prototype.ignore=function(){this.start==this.pos&&(this.pos+=1),this.start=this.pos},R.QueryLexer.prototype.backup=function(){this.pos-=1},R.QueryLexer.prototype.acceptDigitRun=function(){var e,t;do{t=(e=this.next()).charCodeAt(0)}while(t>47&&t<58);e!=R.QueryLexer.EOS&&this.backup()},R.QueryLexer.prototype.more=function(){return this.pos<this.length},R.QueryLexer.EOS="EOS",R.QueryLexer.FIELD="FIELD",R.QueryLexer.TERM="TERM",R.QueryLexer.EDIT_DISTANCE="EDIT_DISTANCE",R.QueryLexer.BOOST="BOOST",R.QueryLexer.PRESENCE="PRESENCE",R.QueryLexer.lexField=function(e){return e.backup(),e.emit(R.QueryLexer.FIELD),e.ignore(),R.QueryLexer.lexText},R.QueryLexer.lexTerm=function(e){if(e.width()>1&&(e.backup(),e.emit(R.QueryLexer.TERM)),e.ignore(),e.more())return R.QueryLexer.lexText},R.QueryLexer.lexEditDistance=function(e){return e.ignore(),e.acceptDigitRun(),e.emit(R.QueryLexer.EDIT_DISTANCE),R.QueryLexer.lexText},R.QueryLexer.lexBoost=function(e){return e.ignore(),e.acceptDigitRun(),e.emit(R.QueryLexer.BOOST),R.QueryLexer.lexText},R.QueryLexer.lexEOS=function(e){e.width()>0&&e.emit(R.QueryLexer.TERM)},R.QueryLexer.termSeparator=R.tokenizer.separator,R.QueryLexer.lexText=function(e){for(;;){var t=e.next();if(t==R.QueryLexer.EOS)return R.QueryLexer.lexEOS;if(92!=t.charCodeAt(0)){if(":"==t)return R.QueryLexer.lexField;if("~"==t)return e.backup(),e.width()>0&&e.emit(R.QueryLexer.TERM),R.QueryLexer.lexEditDistance;if("^"==t)return e.backup(),e.width()>0&&e.emit(R.QueryLexer.TERM),R.QueryLexer.lexBoost;if("+"==t&&1===e.width())return e.emit(R.QueryLexer.PRESENCE),R.QueryLexer.lexText;if("-"==t&&1===e.width())return e.emit(R.QueryLexer.PRESENCE),R.QueryLexer.lexText;if(t.match(R.QueryLexer.termSeparator))return R.QueryLexer.lexTerm}else e.escapeCharacter()}},R.QueryParser=function(e,t){this.lexer=new R.QueryLexer(e),this.query=t,this.currentClause={},this.lexemeIdx=0},R.QueryParser.prototype.parse=function(){this.lexer.run(),this.lexemes=this.lexer.lexemes;for(var e=R.QueryParser.parseClause;e;)e=e(this);return this.query},R.QueryParser.prototype.peekLexeme=function(){return this.lexemes[this.lexemeIdx]},R.QueryParser.prototype.consumeLexeme=function(){var e=this.peekLexeme();return this.lexemeIdx+=1,e},R.QueryParser.prototype.nextClause=function(){var e=this.currentClause;this.query.clause(e),this.currentClause={}},R.QueryParser.parseClause=function(e){var t=e.peekLexeme();if(null!=t)switch(t.type){case R.QueryLexer.PRESENCE:return R.QueryParser.parsePresence;case R.QueryLexer.FIELD:return R.QueryParser.parseField;case R.QueryLexer.TERM:return R.QueryParser.parseTerm;default:var r="expected either a field or a term, found "+t.type;throw t.str.length>=1&&(r+=" with value \'"+t.str+"\'"),new R.QueryParseError(r,t.start,t.end)}},R.QueryParser.parsePresence=function(e){var t=e.consumeLexeme();if(null!=t){switch(t.str){case"-":e.currentClause.presence=R.Query.presence.PROHIBITED;break;case"+":e.currentClause.presence=R.Query.presence.REQUIRED;break;default:var r="unrecognised presence operator\'"+t.str+"\'";throw new R.QueryParseError(r,t.start,t.end)}var n=e.peekLexeme();if(null==n)throw r="expecting term or field, found nothing",new R.QueryParseError(r,t.start,t.end);switch(n.type){case R.QueryLexer.FIELD:return R.QueryParser.parseField;case R.QueryLexer.TERM:return R.QueryParser.parseTerm;default:throw r="expecting term or field, found \'"+n.type+"\'",new R.QueryParseError(r,n.start,n.end)}}},R.QueryParser.parseField=function(e){var t=e.consumeLexeme();if(null!=t){if(-1==e.query.allFields.indexOf(t.str)){var r=e.query.allFields.map((function(e){return"\'"+e+"\'"})).join(", "),n="unrecognised field \'"+t.str+"\', possible fields: "+r;throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.fields=[t.str];var i=e.peekLexeme();if(null==i)throw n="expecting term, found nothing",new R.QueryParseError(n,t.start,t.end);if(i.type===R.QueryLexer.TERM)return R.QueryParser.parseTerm;throw n="expecting term, found \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}},R.QueryParser.parseTerm=function(e){var t=e.consumeLexeme();if(null!=t){e.currentClause.term=t.str.toLowerCase(),-1!=t.str.indexOf("*")&&(e.currentClause.usePipeline=!1);var r=e.peekLexeme();if(null!=r)switch(r.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:var n="Unexpected lexeme type \'"+r.type+"\'";throw new R.QueryParseError(n,r.start,r.end)}else e.nextClause()}},R.QueryParser.parseEditDistance=function(e){var t=e.consumeLexeme();if(null!=t){var r=parseInt(t.str,10);if(isNaN(r)){var n="edit distance must be numeric";throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.editDistance=r;var i=e.peekLexeme();if(null!=i)switch(i.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:throw n="Unexpected lexeme type \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}else e.nextClause()}},R.QueryParser.parseBoost=function(e){var t=e.consumeLexeme();if(null!=t){var r=parseInt(t.str,10);if(isNaN(r)){var n="boost must be numeric";throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.boost=r;var i=e.peekLexeme();if(null!=i)switch(i.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:throw n="Unexpected lexeme type \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}else e.nextClause()}},void 0===(i="function"==typeof(n=function(){return R})?n.call(t,r,t,e):n)||(e.exports=i)}()}},t={};function r(n){var i=t[n];if(void 0!==i)return i.exports;var s=t[n]={exports:{}};return e[n](s,s.exports,r),s.exports}r.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return r.d(t,{a:t}),t},r.d=function(e,t){for(var n in t)r.o(t,n)&&!r.o(e,n)&&Object.defineProperty(e,n,{enumerable:!0,get:t[n]})},r.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)};var n={};!function(){"use strict";r.d(n,{add:function(){return l},dispose:function(){return p},done:function(){return c},fromExternalJS:function(){return d},load:function(){return f},search:function(){return y},toJS:function(){return h}});var e=r(336),t=(e,t,r)=>new Promise(((n,i)=>{var s=e=>{try{a(r.next(e))}catch(e){i(e)}},o=e=>{try{a(r.throw(e))}catch(e){i(e)}},a=e=>e.done?n(e.value):Promise.resolve(e.value).then(s,o);a((r=r.apply(e,t)).next())}));let i,s,o,a=[];function u(){i=new e.Builder,i.field("title"),i.field("description"),i.ref("ref"),i.pipeline.add(e.trimmer,e.stopWordFilter,e.stemmer),o=new Promise((e=>{s=e}))}function l(e,t,r){const n=a.push(r)-1,s={title:e.toLowerCase(),description:t.toLowerCase(),ref:n};i.add(s)}function c(){return t(this,null,(function*(){s(i.build())}))}function h(){return t(this,null,(function*(){return{store:a,index:(yield o).toJSON()}}))}function d(e,r){return t(this,null,(function*(){try{if(importScripts(e),!self[r])throw new Error("Broken index file format");f(self[r])}catch(e){console.error("Failed to load search index: "+e.message)}}))}function f(r){return t(this,null,(function*(){a=r.store,s(e.Index.load(r.index))}))}function p(){return t(this,null,(function*(){a=[],u()}))}function y(r,n=0){return t(this,null,(function*(){if(0===r.trim().length)return[];let t=(yield o).query((t=>{r.trim().toLowerCase().split(/\\s+/).forEach((r=>{if(1===r.length)return;const n=(t=>"*"+e.stemmer(new e.Token(t,{}))+"*")(r);t.term(n,{})}))}));return n>0&&(t=t.slice(0,n)),t.map((e=>({meta:a[e.ref],score:e.score})))}))}e.tokenizer.separator=/\\s+/,u(),addEventListener("message",(function(e){var t,r=e.data,i=r.type,s=r.method,o=r.id,a=r.params;"RPC"===i&&s&&((t=n[s])?Promise.resolve().then((function(){return t.apply(n,a)})):Promise.reject("No such method")).then((function(e){postMessage({type:"RPC",id:o,result:e})})).catch((function(e){var t={message:e};e.stack&&(t.message=e.message,t.stack=e.stack,t.name=e.name),postMessage({type:"RPC",id:o,error:t})}))})),postMessage({type:"RPC",method:"ready"})}()}();\n//# sourceMappingURL=9e68c24da9f5fd56991c.worker.js.map'])), {
+                                var e = new Worker(URL.createObjectURL(new Blob(['/*! For license information please see 0a6ad30060afff00cb34.worker.js.LICENSE.txt */\n!function(){var e={336:function(e,t,r){var n,i;!function(){var s,o,a,u,l,c,h,d,f,p,y,m,g,x,v,w,Q,k,S,E,L,P,b,T,O,I,R=function(e){var t=new R.Builder;return t.pipeline.add(R.trimmer,R.stopWordFilter,R.stemmer),t.searchPipeline.add(R.stemmer),e.call(t,t),t.build()};R.version="2.3.9",R.utils={},R.utils.warn=(s=this,function(e){s.console&&console.warn&&console.warn(e)}),R.utils.asString=function(e){return null==e?"":e.toString()},R.utils.clone=function(e){if(null==e)return e;for(var t=Object.create(null),r=Object.keys(e),n=0;n<r.length;n++){var i=r[n],s=e[i];if(Array.isArray(s))t[i]=s.slice();else{if("string"!=typeof s&&"number"!=typeof s&&"boolean"!=typeof s)throw new TypeError("clone is not deep and does not support nested objects");t[i]=s}}return t},R.FieldRef=function(e,t,r){this.docRef=e,this.fieldName=t,this._stringValue=r},R.FieldRef.joiner="/",R.FieldRef.fromString=function(e){var t=e.indexOf(R.FieldRef.joiner);if(-1===t)throw"malformed field ref string";var r=e.slice(0,t),n=e.slice(t+1);return new R.FieldRef(n,r,e)},R.FieldRef.prototype.toString=function(){return null==this._stringValue&&(this._stringValue=this.fieldName+R.FieldRef.joiner+this.docRef),this._stringValue},R.Set=function(e){if(this.elements=Object.create(null),e){this.length=e.length;for(var t=0;t<this.length;t++)this.elements[e[t]]=!0}else this.length=0},R.Set.complete={intersect:function(e){return e},union:function(){return this},contains:function(){return!0}},R.Set.empty={intersect:function(){return this},union:function(e){return e},contains:function(){return!1}},R.Set.prototype.contains=function(e){return!!this.elements[e]},R.Set.prototype.intersect=function(e){var t,r,n,i=[];if(e===R.Set.complete)return this;if(e===R.Set.empty)return e;this.length<e.length?(t=this,r=e):(t=e,r=this),n=Object.keys(t.elements);for(var s=0;s<n.length;s++){var o=n[s];o in r.elements&&i.push(o)}return new R.Set(i)},R.Set.prototype.union=function(e){return e===R.Set.complete?R.Set.complete:e===R.Set.empty?this:new R.Set(Object.keys(this.elements).concat(Object.keys(e.elements)))},R.idf=function(e,t){var r=0;for(var n in e)"_index"!=n&&(r+=Object.keys(e[n]).length);var i=(t-r+.5)/(r+.5);return Math.log(1+Math.abs(i))},R.Token=function(e,t){this.str=e||"",this.metadata=t||{}},R.Token.prototype.toString=function(){return this.str},R.Token.prototype.update=function(e){return this.str=e(this.str,this.metadata),this},R.Token.prototype.clone=function(e){return e=e||function(e){return e},new R.Token(e(this.str,this.metadata),this.metadata)},R.tokenizer=function(e,t){if(null==e||null==e)return[];if(Array.isArray(e))return e.map((function(e){return new R.Token(R.utils.asString(e).toLowerCase(),R.utils.clone(t))}));for(var r=e.toString().toLowerCase(),n=r.length,i=[],s=0,o=0;s<=n;s++){var a=s-o;if(r.charAt(s).match(R.tokenizer.separator)||s==n){if(a>0){var u=R.utils.clone(t)||{};u.position=[o,a],u.index=i.length,i.push(new R.Token(r.slice(o,s),u))}o=s+1}}return i},R.tokenizer.separator=/[\\s\\-]+/,R.Pipeline=function(){this._stack=[]},R.Pipeline.registeredFunctions=Object.create(null),R.Pipeline.registerFunction=function(e,t){t in this.registeredFunctions&&R.utils.warn("Overwriting existing registered function: "+t),e.label=t,R.Pipeline.registeredFunctions[e.label]=e},R.Pipeline.warnIfFunctionNotRegistered=function(e){e.label&&e.label in this.registeredFunctions||R.utils.warn("Function is not registered with pipeline. This may cause problems when serialising the index.\\n",e)},R.Pipeline.load=function(e){var t=new R.Pipeline;return e.forEach((function(e){var r=R.Pipeline.registeredFunctions[e];if(!r)throw new Error("Cannot load unregistered function: "+e);t.add(r)})),t},R.Pipeline.prototype.add=function(){var e=Array.prototype.slice.call(arguments);e.forEach((function(e){R.Pipeline.warnIfFunctionNotRegistered(e),this._stack.push(e)}),this)},R.Pipeline.prototype.after=function(e,t){R.Pipeline.warnIfFunctionNotRegistered(t);var r=this._stack.indexOf(e);if(-1==r)throw new Error("Cannot find existingFn");r+=1,this._stack.splice(r,0,t)},R.Pipeline.prototype.before=function(e,t){R.Pipeline.warnIfFunctionNotRegistered(t);var r=this._stack.indexOf(e);if(-1==r)throw new Error("Cannot find existingFn");this._stack.splice(r,0,t)},R.Pipeline.prototype.remove=function(e){var t=this._stack.indexOf(e);-1!=t&&this._stack.splice(t,1)},R.Pipeline.prototype.run=function(e){for(var t=this._stack.length,r=0;r<t;r++){for(var n=this._stack[r],i=[],s=0;s<e.length;s++){var o=n(e[s],s,e);if(null!=o&&""!==o)if(Array.isArray(o))for(var a=0;a<o.length;a++)i.push(o[a]);else i.push(o)}e=i}return e},R.Pipeline.prototype.runString=function(e,t){var r=new R.Token(e,t);return this.run([r]).map((function(e){return e.toString()}))},R.Pipeline.prototype.reset=function(){this._stack=[]},R.Pipeline.prototype.toJSON=function(){return this._stack.map((function(e){return R.Pipeline.warnIfFunctionNotRegistered(e),e.label}))},R.Vector=function(e){this._magnitude=0,this.elements=e||[]},R.Vector.prototype.positionForIndex=function(e){if(0==this.elements.length)return 0;for(var t=0,r=this.elements.length/2,n=r-t,i=Math.floor(n/2),s=this.elements[2*i];n>1&&(s<e&&(t=i),s>e&&(r=i),s!=e);)n=r-t,i=t+Math.floor(n/2),s=this.elements[2*i];return s==e||s>e?2*i:s<e?2*(i+1):void 0},R.Vector.prototype.insert=function(e,t){this.upsert(e,t,(function(){throw"duplicate index"}))},R.Vector.prototype.upsert=function(e,t,r){this._magnitude=0;var n=this.positionForIndex(e);this.elements[n]==e?this.elements[n+1]=r(this.elements[n+1],t):this.elements.splice(n,0,e,t)},R.Vector.prototype.magnitude=function(){if(this._magnitude)return this._magnitude;for(var e=0,t=this.elements.length,r=1;r<t;r+=2){var n=this.elements[r];e+=n*n}return this._magnitude=Math.sqrt(e)},R.Vector.prototype.dot=function(e){for(var t=0,r=this.elements,n=e.elements,i=r.length,s=n.length,o=0,a=0,u=0,l=0;u<i&&l<s;)(o=r[u])<(a=n[l])?u+=2:o>a?l+=2:o==a&&(t+=r[u+1]*n[l+1],u+=2,l+=2);return t},R.Vector.prototype.similarity=function(e){return this.dot(e)/this.magnitude()||0},R.Vector.prototype.toArray=function(){for(var e=new Array(this.elements.length/2),t=1,r=0;t<this.elements.length;t+=2,r++)e[r]=this.elements[t];return e},R.Vector.prototype.toJSON=function(){return this.elements},R.stemmer=(o={ational:"ate",tional:"tion",enci:"ence",anci:"ance",izer:"ize",bli:"ble",alli:"al",entli:"ent",eli:"e",ousli:"ous",ization:"ize",ation:"ate",ator:"ate",alism:"al",iveness:"ive",fulness:"ful",ousness:"ous",aliti:"al",iviti:"ive",biliti:"ble",logi:"log"},a={icate:"ic",ative:"",alize:"al",iciti:"ic",ical:"ic",ful:"",ness:""},u="[aeiouy]",l="[^aeiou][^aeiouy]*",c=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*"),h=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*[aeiouy][aeiou]*[^aeiou][^aeiouy]*"),d=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy][aeiou]*[^aeiou][^aeiouy]*([aeiouy][aeiou]*)?$"),f=new RegExp("^([^aeiou][^aeiouy]*)?[aeiouy]"),p=/^(.+?)(ss|i)es$/,y=/^(.+?)([^s])s$/,m=/^(.+?)eed$/,g=/^(.+?)(ed|ing)$/,x=/.$/,v=/(at|bl|iz)$/,w=new RegExp("([^aeiouylsz])\\\\1$"),Q=new RegExp("^"+l+u+"[^aeiouwxy]$"),k=/^(.+?[^aeiou])y$/,S=/^(.+?)(ational|tional|enci|anci|izer|bli|alli|entli|eli|ousli|ization|ation|ator|alism|iveness|fulness|ousness|aliti|iviti|biliti|logi)$/,E=/^(.+?)(icate|ative|alize|iciti|ical|ful|ness)$/,L=/^(.+?)(al|ance|ence|er|ic|able|ible|ant|ement|ment|ent|ou|ism|ate|iti|ous|ive|ize)$/,P=/^(.+?)(s|t)(ion)$/,b=/^(.+?)e$/,T=/ll$/,O=new RegExp("^"+l+u+"[^aeiouwxy]$"),I=function(e){var t,r,n,i,s,u,l;if(e.length<3)return e;if("y"==(n=e.substr(0,1))&&(e=n.toUpperCase()+e.substr(1)),s=y,(i=p).test(e)?e=e.replace(i,"$1$2"):s.test(e)&&(e=e.replace(s,"$1$2")),s=g,(i=m).test(e)){var I=i.exec(e);(i=c).test(I[1])&&(i=x,e=e.replace(i,""))}else s.test(e)&&(t=(I=s.exec(e))[1],(s=f).test(t)&&(u=w,l=Q,(s=v).test(e=t)?e+="e":u.test(e)?(i=x,e=e.replace(i,"")):l.test(e)&&(e+="e")));return(i=k).test(e)&&(e=(t=(I=i.exec(e))[1])+"i"),(i=S).test(e)&&(t=(I=i.exec(e))[1],r=I[2],(i=c).test(t)&&(e=t+o[r])),(i=E).test(e)&&(t=(I=i.exec(e))[1],r=I[2],(i=c).test(t)&&(e=t+a[r])),s=P,(i=L).test(e)?(t=(I=i.exec(e))[1],(i=h).test(t)&&(e=t)):s.test(e)&&(t=(I=s.exec(e))[1]+I[2],(s=h).test(t)&&(e=t)),(i=b).test(e)&&(t=(I=i.exec(e))[1],s=d,u=O,((i=h).test(t)||s.test(t)&&!u.test(t))&&(e=t)),s=h,(i=T).test(e)&&s.test(e)&&(i=x,e=e.replace(i,"")),"y"==n&&(e=n.toLowerCase()+e.substr(1)),e},function(e){return e.update(I)}),R.Pipeline.registerFunction(R.stemmer,"stemmer"),R.generateStopWordFilter=function(e){var t=e.reduce((function(e,t){return e[t]=t,e}),{});return function(e){if(e&&t[e.toString()]!==e.toString())return e}},R.stopWordFilter=R.generateStopWordFilter(["a","able","about","across","after","all","almost","also","am","among","an","and","any","are","as","at","be","because","been","but","by","can","cannot","could","dear","did","do","does","either","else","ever","every","for","from","get","got","had","has","have","he","her","hers","him","his","how","however","i","if","in","into","is","it","its","just","least","let","like","likely","may","me","might","most","must","my","neither","no","nor","not","of","off","often","on","only","or","other","our","own","rather","said","say","says","she","should","since","so","some","than","that","the","their","them","then","there","these","they","this","tis","to","too","twas","us","wants","was","we","were","what","when","where","which","while","who","whom","why","will","with","would","yet","you","your"]),R.Pipeline.registerFunction(R.stopWordFilter,"stopWordFilter"),R.trimmer=function(e){return e.update((function(e){return e.replace(/^\\W+/,"").replace(/\\W+$/,"")}))},R.Pipeline.registerFunction(R.trimmer,"trimmer"),R.TokenSet=function(){this.final=!1,this.edges={},this.id=R.TokenSet._nextId,R.TokenSet._nextId+=1},R.TokenSet._nextId=1,R.TokenSet.fromArray=function(e){for(var t=new R.TokenSet.Builder,r=0,n=e.length;r<n;r++)t.insert(e[r]);return t.finish(),t.root},R.TokenSet.fromClause=function(e){return"editDistance"in e?R.TokenSet.fromFuzzyString(e.term,e.editDistance):R.TokenSet.fromString(e.term)},R.TokenSet.fromFuzzyString=function(e,t){for(var r=new R.TokenSet,n=[{node:r,editsRemaining:t,str:e}];n.length;){var i=n.pop();if(i.str.length>0){var s,o=i.str.charAt(0);o in i.node.edges?s=i.node.edges[o]:(s=new R.TokenSet,i.node.edges[o]=s),1==i.str.length&&(s.final=!0),n.push({node:s,editsRemaining:i.editsRemaining,str:i.str.slice(1)})}if(0!=i.editsRemaining){if("*"in i.node.edges)var a=i.node.edges["*"];else a=new R.TokenSet,i.node.edges["*"]=a;if(0==i.str.length&&(a.final=!0),n.push({node:a,editsRemaining:i.editsRemaining-1,str:i.str}),i.str.length>1&&n.push({node:i.node,editsRemaining:i.editsRemaining-1,str:i.str.slice(1)}),1==i.str.length&&(i.node.final=!0),i.str.length>=1){if("*"in i.node.edges)var u=i.node.edges["*"];else u=new R.TokenSet,i.node.edges["*"]=u;1==i.str.length&&(u.final=!0),n.push({node:u,editsRemaining:i.editsRemaining-1,str:i.str.slice(1)})}if(i.str.length>1){var l,c=i.str.charAt(0),h=i.str.charAt(1);h in i.node.edges?l=i.node.edges[h]:(l=new R.TokenSet,i.node.edges[h]=l),1==i.str.length&&(l.final=!0),n.push({node:l,editsRemaining:i.editsRemaining-1,str:c+i.str.slice(2)})}}}return r},R.TokenSet.fromString=function(e){for(var t=new R.TokenSet,r=t,n=0,i=e.length;n<i;n++){var s=e[n],o=n==i-1;if("*"==s)t.edges[s]=t,t.final=o;else{var a=new R.TokenSet;a.final=o,t.edges[s]=a,t=a}}return r},R.TokenSet.prototype.toArray=function(){for(var e=[],t=[{prefix:"",node:this}];t.length;){var r=t.pop(),n=Object.keys(r.node.edges),i=n.length;r.node.final&&(r.prefix.charAt(0),e.push(r.prefix));for(var s=0;s<i;s++){var o=n[s];t.push({prefix:r.prefix.concat(o),node:r.node.edges[o]})}}return e},R.TokenSet.prototype.toString=function(){if(this._str)return this._str;for(var e=this.final?"1":"0",t=Object.keys(this.edges).sort(),r=t.length,n=0;n<r;n++){var i=t[n];e=e+i+this.edges[i].id}return e},R.TokenSet.prototype.intersect=function(e){for(var t=new R.TokenSet,r=void 0,n=[{qNode:e,output:t,node:this}];n.length;){r=n.pop();for(var i=Object.keys(r.qNode.edges),s=i.length,o=Object.keys(r.node.edges),a=o.length,u=0;u<s;u++)for(var l=i[u],c=0;c<a;c++){var h=o[c];if(h==l||"*"==l){var d=r.node.edges[h],f=r.qNode.edges[l],p=d.final&&f.final,y=void 0;h in r.output.edges?(y=r.output.edges[h]).final=y.final||p:((y=new R.TokenSet).final=p,r.output.edges[h]=y),n.push({qNode:f,output:y,node:d})}}}return t},R.TokenSet.Builder=function(){this.previousWord="",this.root=new R.TokenSet,this.uncheckedNodes=[],this.minimizedNodes={}},R.TokenSet.Builder.prototype.insert=function(e){var t,r=0;if(e<this.previousWord)throw new Error("Out of order word insertion");for(var n=0;n<e.length&&n<this.previousWord.length&&e[n]==this.previousWord[n];n++)r++;for(this.minimize(r),t=0==this.uncheckedNodes.length?this.root:this.uncheckedNodes[this.uncheckedNodes.length-1].child,n=r;n<e.length;n++){var i=new R.TokenSet,s=e[n];t.edges[s]=i,this.uncheckedNodes.push({parent:t,char:s,child:i}),t=i}t.final=!0,this.previousWord=e},R.TokenSet.Builder.prototype.finish=function(){this.minimize(0)},R.TokenSet.Builder.prototype.minimize=function(e){for(var t=this.uncheckedNodes.length-1;t>=e;t--){var r=this.uncheckedNodes[t],n=r.child.toString();n in this.minimizedNodes?r.parent.edges[r.char]=this.minimizedNodes[n]:(r.child._str=n,this.minimizedNodes[n]=r.child),this.uncheckedNodes.pop()}},R.Index=function(e){this.invertedIndex=e.invertedIndex,this.fieldVectors=e.fieldVectors,this.tokenSet=e.tokenSet,this.fields=e.fields,this.pipeline=e.pipeline},R.Index.prototype.search=function(e){return this.query((function(t){new R.QueryParser(e,t).parse()}))},R.Index.prototype.query=function(e){for(var t=new R.Query(this.fields),r=Object.create(null),n=Object.create(null),i=Object.create(null),s=Object.create(null),o=Object.create(null),a=0;a<this.fields.length;a++)n[this.fields[a]]=new R.Vector;for(e.call(t,t),a=0;a<t.clauses.length;a++){var u,l=t.clauses[a],c=R.Set.empty;u=l.usePipeline?this.pipeline.runString(l.term,{fields:l.fields}):[l.term];for(var h=0;h<u.length;h++){var d=u[h];l.term=d;var f=R.TokenSet.fromClause(l),p=this.tokenSet.intersect(f).toArray();if(0===p.length&&l.presence===R.Query.presence.REQUIRED){for(var y=0;y<l.fields.length;y++)s[F=l.fields[y]]=R.Set.empty;break}for(var m=0;m<p.length;m++){var g=p[m],x=this.invertedIndex[g],v=x._index;for(y=0;y<l.fields.length;y++){var w=x[F=l.fields[y]],Q=Object.keys(w),k=g+"/"+F,S=new R.Set(Q);if(l.presence==R.Query.presence.REQUIRED&&(c=c.union(S),void 0===s[F]&&(s[F]=R.Set.complete)),l.presence!=R.Query.presence.PROHIBITED){if(n[F].upsert(v,l.boost,(function(e,t){return e+t})),!i[k]){for(var E=0;E<Q.length;E++){var L,P=Q[E],b=new R.FieldRef(P,F),T=w[P];void 0===(L=r[b])?r[b]=new R.MatchData(g,F,T):L.add(g,F,T)}i[k]=!0}}else void 0===o[F]&&(o[F]=R.Set.empty),o[F]=o[F].union(S)}}}if(l.presence===R.Query.presence.REQUIRED)for(y=0;y<l.fields.length;y++)s[F=l.fields[y]]=s[F].intersect(c)}var O=R.Set.complete,I=R.Set.empty;for(a=0;a<this.fields.length;a++){var F;s[F=this.fields[a]]&&(O=O.intersect(s[F])),o[F]&&(I=I.union(o[F]))}var C=Object.keys(r),N=[],j=Object.create(null);if(t.isNegated())for(C=Object.keys(this.fieldVectors),a=0;a<C.length;a++){b=C[a];var _=R.FieldRef.fromString(b);r[b]=new R.MatchData}for(a=0;a<C.length;a++){var D=(_=R.FieldRef.fromString(C[a])).docRef;if(O.contains(D)&&!I.contains(D)){var A,B=this.fieldVectors[_],z=n[_.fieldName].similarity(B);if(void 0!==(A=j[D]))A.score+=z,A.matchData.combine(r[_]);else{var V={ref:D,score:z,matchData:r[_]};j[D]=V,N.push(V)}}}return N.sort((function(e,t){return t.score-e.score}))},R.Index.prototype.toJSON=function(){var e=Object.keys(this.invertedIndex).sort().map((function(e){return[e,this.invertedIndex[e]]}),this),t=Object.keys(this.fieldVectors).map((function(e){return[e,this.fieldVectors[e].toJSON()]}),this);return{version:R.version,fields:this.fields,fieldVectors:t,invertedIndex:e,pipeline:this.pipeline.toJSON()}},R.Index.load=function(e){var t={},r={},n=e.fieldVectors,i=Object.create(null),s=e.invertedIndex,o=new R.TokenSet.Builder,a=R.Pipeline.load(e.pipeline);e.version!=R.version&&R.utils.warn("Version mismatch when loading serialised index. Current version of lunr \'"+R.version+"\' does not match serialized index \'"+e.version+"\'");for(var u=0;u<n.length;u++){var l=(h=n[u])[0],c=h[1];r[l]=new R.Vector(c)}for(u=0;u<s.length;u++){var h,d=(h=s[u])[0],f=h[1];o.insert(d),i[d]=f}return o.finish(),t.fields=e.fields,t.fieldVectors=r,t.invertedIndex=i,t.tokenSet=o.root,t.pipeline=a,new R.Index(t)},R.Builder=function(){this._ref="id",this._fields=Object.create(null),this._documents=Object.create(null),this.invertedIndex=Object.create(null),this.fieldTermFrequencies={},this.fieldLengths={},this.tokenizer=R.tokenizer,this.pipeline=new R.Pipeline,this.searchPipeline=new R.Pipeline,this.documentCount=0,this._b=.75,this._k1=1.2,this.termIndex=0,this.metadataWhitelist=[]},R.Builder.prototype.ref=function(e){this._ref=e},R.Builder.prototype.field=function(e,t){if(/\\//.test(e))throw new RangeError("Field \'"+e+"\' contains illegal character \'/\'");this._fields[e]=t||{}},R.Builder.prototype.b=function(e){this._b=e<0?0:e>1?1:e},R.Builder.prototype.k1=function(e){this._k1=e},R.Builder.prototype.add=function(e,t){var r=e[this._ref],n=Object.keys(this._fields);this._documents[r]=t||{},this.documentCount+=1;for(var i=0;i<n.length;i++){var s=n[i],o=this._fields[s].extractor,a=o?o(e):e[s],u=this.tokenizer(a,{fields:[s]}),l=this.pipeline.run(u),c=new R.FieldRef(r,s),h=Object.create(null);this.fieldTermFrequencies[c]=h,this.fieldLengths[c]=0,this.fieldLengths[c]+=l.length;for(var d=0;d<l.length;d++){var f=l[d];if(null==h[f]&&(h[f]=0),h[f]+=1,null==this.invertedIndex[f]){var p=Object.create(null);p._index=this.termIndex,this.termIndex+=1;for(var y=0;y<n.length;y++)p[n[y]]=Object.create(null);this.invertedIndex[f]=p}null==this.invertedIndex[f][s][r]&&(this.invertedIndex[f][s][r]=Object.create(null));for(var m=0;m<this.metadataWhitelist.length;m++){var g=this.metadataWhitelist[m],x=f.metadata[g];null==this.invertedIndex[f][s][r][g]&&(this.invertedIndex[f][s][r][g]=[]),this.invertedIndex[f][s][r][g].push(x)}}}},R.Builder.prototype.calculateAverageFieldLengths=function(){for(var e=Object.keys(this.fieldLengths),t=e.length,r={},n={},i=0;i<t;i++){var s=R.FieldRef.fromString(e[i]),o=s.fieldName;n[o]||(n[o]=0),n[o]+=1,r[o]||(r[o]=0),r[o]+=this.fieldLengths[s]}var a=Object.keys(this._fields);for(i=0;i<a.length;i++){var u=a[i];r[u]=r[u]/n[u]}this.averageFieldLength=r},R.Builder.prototype.createFieldVectors=function(){for(var e={},t=Object.keys(this.fieldTermFrequencies),r=t.length,n=Object.create(null),i=0;i<r;i++){for(var s=R.FieldRef.fromString(t[i]),o=s.fieldName,a=this.fieldLengths[s],u=new R.Vector,l=this.fieldTermFrequencies[s],c=Object.keys(l),h=c.length,d=this._fields[o].boost||1,f=this._documents[s.docRef].boost||1,p=0;p<h;p++){var y,m,g,x=c[p],v=l[x],w=this.invertedIndex[x]._index;void 0===n[x]?(y=R.idf(this.invertedIndex[x],this.documentCount),n[x]=y):y=n[x],m=y*((this._k1+1)*v)/(this._k1*(1-this._b+this._b*(a/this.averageFieldLength[o]))+v),m*=d,m*=f,g=Math.round(1e3*m)/1e3,u.insert(w,g)}e[s]=u}this.fieldVectors=e},R.Builder.prototype.createTokenSet=function(){this.tokenSet=R.TokenSet.fromArray(Object.keys(this.invertedIndex).sort())},R.Builder.prototype.build=function(){return this.calculateAverageFieldLengths(),this.createFieldVectors(),this.createTokenSet(),new R.Index({invertedIndex:this.invertedIndex,fieldVectors:this.fieldVectors,tokenSet:this.tokenSet,fields:Object.keys(this._fields),pipeline:this.searchPipeline})},R.Builder.prototype.use=function(e){var t=Array.prototype.slice.call(arguments,1);t.unshift(this),e.apply(this,t)},R.MatchData=function(e,t,r){for(var n=Object.create(null),i=Object.keys(r||{}),s=0;s<i.length;s++){var o=i[s];n[o]=r[o].slice()}this.metadata=Object.create(null),void 0!==e&&(this.metadata[e]=Object.create(null),this.metadata[e][t]=n)},R.MatchData.prototype.combine=function(e){for(var t=Object.keys(e.metadata),r=0;r<t.length;r++){var n=t[r],i=Object.keys(e.metadata[n]);null==this.metadata[n]&&(this.metadata[n]=Object.create(null));for(var s=0;s<i.length;s++){var o=i[s],a=Object.keys(e.metadata[n][o]);null==this.metadata[n][o]&&(this.metadata[n][o]=Object.create(null));for(var u=0;u<a.length;u++){var l=a[u];null==this.metadata[n][o][l]?this.metadata[n][o][l]=e.metadata[n][o][l]:this.metadata[n][o][l]=this.metadata[n][o][l].concat(e.metadata[n][o][l])}}}},R.MatchData.prototype.add=function(e,t,r){if(!(e in this.metadata))return this.metadata[e]=Object.create(null),void(this.metadata[e][t]=r);if(t in this.metadata[e])for(var n=Object.keys(r),i=0;i<n.length;i++){var s=n[i];s in this.metadata[e][t]?this.metadata[e][t][s]=this.metadata[e][t][s].concat(r[s]):this.metadata[e][t][s]=r[s]}else this.metadata[e][t]=r},R.Query=function(e){this.clauses=[],this.allFields=e},R.Query.wildcard=new String("*"),R.Query.wildcard.NONE=0,R.Query.wildcard.LEADING=1,R.Query.wildcard.TRAILING=2,R.Query.presence={OPTIONAL:1,REQUIRED:2,PROHIBITED:3},R.Query.prototype.clause=function(e){return"fields"in e||(e.fields=this.allFields),"boost"in e||(e.boost=1),"usePipeline"in e||(e.usePipeline=!0),"wildcard"in e||(e.wildcard=R.Query.wildcard.NONE),e.wildcard&R.Query.wildcard.LEADING&&e.term.charAt(0)!=R.Query.wildcard&&(e.term="*"+e.term),e.wildcard&R.Query.wildcard.TRAILING&&e.term.slice(-1)!=R.Query.wildcard&&(e.term=e.term+"*"),"presence"in e||(e.presence=R.Query.presence.OPTIONAL),this.clauses.push(e),this},R.Query.prototype.isNegated=function(){for(var e=0;e<this.clauses.length;e++)if(this.clauses[e].presence!=R.Query.presence.PROHIBITED)return!1;return!0},R.Query.prototype.term=function(e,t){if(Array.isArray(e))return e.forEach((function(e){this.term(e,R.utils.clone(t))}),this),this;var r=t||{};return r.term=e.toString(),this.clause(r),this},R.QueryParseError=function(e,t,r){this.name="QueryParseError",this.message=e,this.start=t,this.end=r},R.QueryParseError.prototype=new Error,R.QueryLexer=function(e){this.lexemes=[],this.str=e,this.length=e.length,this.pos=0,this.start=0,this.escapeCharPositions=[]},R.QueryLexer.prototype.run=function(){for(var e=R.QueryLexer.lexText;e;)e=e(this)},R.QueryLexer.prototype.sliceString=function(){for(var e=[],t=this.start,r=this.pos,n=0;n<this.escapeCharPositions.length;n++)r=this.escapeCharPositions[n],e.push(this.str.slice(t,r)),t=r+1;return e.push(this.str.slice(t,this.pos)),this.escapeCharPositions.length=0,e.join("")},R.QueryLexer.prototype.emit=function(e){this.lexemes.push({type:e,str:this.sliceString(),start:this.start,end:this.pos}),this.start=this.pos},R.QueryLexer.prototype.escapeCharacter=function(){this.escapeCharPositions.push(this.pos-1),this.pos+=1},R.QueryLexer.prototype.next=function(){if(this.pos>=this.length)return R.QueryLexer.EOS;var e=this.str.charAt(this.pos);return this.pos+=1,e},R.QueryLexer.prototype.width=function(){return this.pos-this.start},R.QueryLexer.prototype.ignore=function(){this.start==this.pos&&(this.pos+=1),this.start=this.pos},R.QueryLexer.prototype.backup=function(){this.pos-=1},R.QueryLexer.prototype.acceptDigitRun=function(){var e,t;do{t=(e=this.next()).charCodeAt(0)}while(t>47&&t<58);e!=R.QueryLexer.EOS&&this.backup()},R.QueryLexer.prototype.more=function(){return this.pos<this.length},R.QueryLexer.EOS="EOS",R.QueryLexer.FIELD="FIELD",R.QueryLexer.TERM="TERM",R.QueryLexer.EDIT_DISTANCE="EDIT_DISTANCE",R.QueryLexer.BOOST="BOOST",R.QueryLexer.PRESENCE="PRESENCE",R.QueryLexer.lexField=function(e){return e.backup(),e.emit(R.QueryLexer.FIELD),e.ignore(),R.QueryLexer.lexText},R.QueryLexer.lexTerm=function(e){if(e.width()>1&&(e.backup(),e.emit(R.QueryLexer.TERM)),e.ignore(),e.more())return R.QueryLexer.lexText},R.QueryLexer.lexEditDistance=function(e){return e.ignore(),e.acceptDigitRun(),e.emit(R.QueryLexer.EDIT_DISTANCE),R.QueryLexer.lexText},R.QueryLexer.lexBoost=function(e){return e.ignore(),e.acceptDigitRun(),e.emit(R.QueryLexer.BOOST),R.QueryLexer.lexText},R.QueryLexer.lexEOS=function(e){e.width()>0&&e.emit(R.QueryLexer.TERM)},R.QueryLexer.termSeparator=R.tokenizer.separator,R.QueryLexer.lexText=function(e){for(;;){var t=e.next();if(t==R.QueryLexer.EOS)return R.QueryLexer.lexEOS;if(92!=t.charCodeAt(0)){if(":"==t)return R.QueryLexer.lexField;if("~"==t)return e.backup(),e.width()>0&&e.emit(R.QueryLexer.TERM),R.QueryLexer.lexEditDistance;if("^"==t)return e.backup(),e.width()>0&&e.emit(R.QueryLexer.TERM),R.QueryLexer.lexBoost;if("+"==t&&1===e.width())return e.emit(R.QueryLexer.PRESENCE),R.QueryLexer.lexText;if("-"==t&&1===e.width())return e.emit(R.QueryLexer.PRESENCE),R.QueryLexer.lexText;if(t.match(R.QueryLexer.termSeparator))return R.QueryLexer.lexTerm}else e.escapeCharacter()}},R.QueryParser=function(e,t){this.lexer=new R.QueryLexer(e),this.query=t,this.currentClause={},this.lexemeIdx=0},R.QueryParser.prototype.parse=function(){this.lexer.run(),this.lexemes=this.lexer.lexemes;for(var e=R.QueryParser.parseClause;e;)e=e(this);return this.query},R.QueryParser.prototype.peekLexeme=function(){return this.lexemes[this.lexemeIdx]},R.QueryParser.prototype.consumeLexeme=function(){var e=this.peekLexeme();return this.lexemeIdx+=1,e},R.QueryParser.prototype.nextClause=function(){var e=this.currentClause;this.query.clause(e),this.currentClause={}},R.QueryParser.parseClause=function(e){var t=e.peekLexeme();if(null!=t)switch(t.type){case R.QueryLexer.PRESENCE:return R.QueryParser.parsePresence;case R.QueryLexer.FIELD:return R.QueryParser.parseField;case R.QueryLexer.TERM:return R.QueryParser.parseTerm;default:var r="expected either a field or a term, found "+t.type;throw t.str.length>=1&&(r+=" with value \'"+t.str+"\'"),new R.QueryParseError(r,t.start,t.end)}},R.QueryParser.parsePresence=function(e){var t=e.consumeLexeme();if(null!=t){switch(t.str){case"-":e.currentClause.presence=R.Query.presence.PROHIBITED;break;case"+":e.currentClause.presence=R.Query.presence.REQUIRED;break;default:var r="unrecognised presence operator\'"+t.str+"\'";throw new R.QueryParseError(r,t.start,t.end)}var n=e.peekLexeme();if(null==n)throw r="expecting term or field, found nothing",new R.QueryParseError(r,t.start,t.end);switch(n.type){case R.QueryLexer.FIELD:return R.QueryParser.parseField;case R.QueryLexer.TERM:return R.QueryParser.parseTerm;default:throw r="expecting term or field, found \'"+n.type+"\'",new R.QueryParseError(r,n.start,n.end)}}},R.QueryParser.parseField=function(e){var t=e.consumeLexeme();if(null!=t){if(-1==e.query.allFields.indexOf(t.str)){var r=e.query.allFields.map((function(e){return"\'"+e+"\'"})).join(", "),n="unrecognised field \'"+t.str+"\', possible fields: "+r;throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.fields=[t.str];var i=e.peekLexeme();if(null==i)throw n="expecting term, found nothing",new R.QueryParseError(n,t.start,t.end);if(i.type===R.QueryLexer.TERM)return R.QueryParser.parseTerm;throw n="expecting term, found \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}},R.QueryParser.parseTerm=function(e){var t=e.consumeLexeme();if(null!=t){e.currentClause.term=t.str.toLowerCase(),-1!=t.str.indexOf("*")&&(e.currentClause.usePipeline=!1);var r=e.peekLexeme();if(null!=r)switch(r.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:var n="Unexpected lexeme type \'"+r.type+"\'";throw new R.QueryParseError(n,r.start,r.end)}else e.nextClause()}},R.QueryParser.parseEditDistance=function(e){var t=e.consumeLexeme();if(null!=t){var r=parseInt(t.str,10);if(isNaN(r)){var n="edit distance must be numeric";throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.editDistance=r;var i=e.peekLexeme();if(null!=i)switch(i.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:throw n="Unexpected lexeme type \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}else e.nextClause()}},R.QueryParser.parseBoost=function(e){var t=e.consumeLexeme();if(null!=t){var r=parseInt(t.str,10);if(isNaN(r)){var n="boost must be numeric";throw new R.QueryParseError(n,t.start,t.end)}e.currentClause.boost=r;var i=e.peekLexeme();if(null!=i)switch(i.type){case R.QueryLexer.TERM:return e.nextClause(),R.QueryParser.parseTerm;case R.QueryLexer.FIELD:return e.nextClause(),R.QueryParser.parseField;case R.QueryLexer.EDIT_DISTANCE:return R.QueryParser.parseEditDistance;case R.QueryLexer.BOOST:return R.QueryParser.parseBoost;case R.QueryLexer.PRESENCE:return e.nextClause(),R.QueryParser.parsePresence;default:throw n="Unexpected lexeme type \'"+i.type+"\'",new R.QueryParseError(n,i.start,i.end)}else e.nextClause()}},void 0===(i="function"==typeof(n=function(){return R})?n.call(t,r,t,e):n)||(e.exports=i)}()}},t={};function r(n){var i=t[n];if(void 0!==i)return i.exports;var s=t[n]={exports:{}};return e[n](s,s.exports,r),s.exports}r.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return r.d(t,{a:t}),t},r.d=function(e,t){for(var n in t)r.o(t,n)&&!r.o(e,n)&&Object.defineProperty(e,n,{enumerable:!0,get:t[n]})},r.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)};var n={};!function(){"use strict";r.d(n,{add:function(){return l},dispose:function(){return p},done:function(){return c},fromExternalJS:function(){return d},load:function(){return f},search:function(){return y},toJS:function(){return h}});var e=r(336),t=(e,t,r)=>new Promise(((n,i)=>{var s=e=>{try{a(r.next(e))}catch(e){i(e)}},o=e=>{try{a(r.throw(e))}catch(e){i(e)}},a=e=>e.done?n(e.value):Promise.resolve(e.value).then(s,o);a((r=r.apply(e,t)).next())}));let i,s,o,a=[];function u(){i=new e.Builder,i.field("title"),i.field("description"),i.ref("ref"),i.pipeline.add(e.trimmer,e.stopWordFilter,e.stemmer),o=new Promise((e=>{s=e}))}function l(e,t,r){const n=a.push(r)-1,s={title:e.toLowerCase(),description:t.toLowerCase(),ref:n};i.add(s)}function c(){return t(this,null,(function*(){s(i.build())}))}function h(){return t(this,null,(function*(){return{store:a,index:(yield o).toJSON()}}))}function d(e,r){return t(this,null,(function*(){try{if(importScripts(e),!self[r])throw new Error("Broken index file format");f(self[r])}catch(e){console.error("Failed to load search index: "+e.message)}}))}function f(r){return t(this,null,(function*(){a=r.store,s(e.Index.load(r.index))}))}function p(){return t(this,null,(function*(){a=[],u()}))}function y(r,n=0){return t(this,null,(function*(){if(0===r.trim().length)return[];let t=(yield o).query((t=>{r.trim().toLowerCase().split(/\\s+/).forEach((r=>{if(1===r.length)return;const n=(t=>{const r=e.trimmer(new e.Token(t,{}));return"*"+e.stemmer(r)+"*"})(r);t.term(n,{})}))}));return n>0&&(t=t.slice(0,n)),t.map((e=>({meta:a[e.ref],score:e.score})))}))}e.tokenizer.separator=/\\s+/,u(),addEventListener("message",(function(e){var t,r=e.data,i=r.type,s=r.method,o=r.id,a=r.params;"RPC"===i&&s&&((t=n[s])?Promise.resolve().then((function(){return t.apply(n,a)})):Promise.reject("No such method")).then((function(e){postMessage({type:"RPC",id:o,result:e})})).catch((function(e){var t={message:e};e.stack&&(t.message=e.message,t.stack=e.stack,t.name=e.name),postMessage({type:"RPC",id:o,error:t})}))})),postMessage({type:"RPC",method:"ready"})}()}();\n//# sourceMappingURL=0a6ad30060afff00cb34.worker.js.map'])), {
                                     name: "[fullhash].worker.js"
                                 });
                                 return r(e, o), e
                             }
                         },
                         6314: function(e) {
                             e.exports = function(e, t) {
@@ -32176,15 +32176,15 @@
                             }
                             componentDidCatch(e) {
                                 return this.setState({
                                     error: e
                                 }), !1
                             }
                             render() {
-                                return this.state.error ? n.createElement(va, null, n.createElement("h1", null, "Something went wrong..."), n.createElement("small", null, " ", this.state.error.message, " "), n.createElement("p", null, n.createElement("details", null, n.createElement("summary", null, "Stack trace"), n.createElement("pre", null, this.state.error.stack))), n.createElement("small", null, " ReDoc Version: ", "2.0.0-rc.75"), " ", n.createElement("br", null), n.createElement("small", null, " Commit: ", "d7440fb")) : n.createElement(n.Fragment, null, n.Children.only(this.props.children))
+                                return this.state.error ? n.createElement(va, null, n.createElement("h1", null, "Something went wrong..."), n.createElement("small", null, " ", this.state.error.message, " "), n.createElement("p", null, n.createElement("details", null, n.createElement("summary", null, "Stack trace"), n.createElement("pre", null, this.state.error.stack))), n.createElement("small", null, " ReDoc Version: ", "2.0.0"), " ", n.createElement("br", null), n.createElement("small", null, " Commit: ", "5fb4daa")) : n.createElement(n.Fragment, null, n.Children.only(this.props.children))
                             }
                         }
                         const wa = fa`
   0% {
     transform: rotate(0deg); }
   100% {
     transform: rotate(360deg);
@@ -33912,28 +33912,28 @@
                         const Cl = new wl.Renderer;
                         wl.setOptions({
                             renderer: Cl,
                             highlight: (e, t) => vs(e, t)
                         });
                         const Rl = "(?:^ {0,3}\x3c!-- ReDoc-Inject:\\s+?<({component}).*?/?>\\s+?--\x3e\\s*$|(?:^ {0,3}<({component})([\\s\\S]*?)>([\\s\\S]*?)</\\2>|^ {0,3}<({component})([\\s\\S]*?)(?:/>|\\n{2,})))";
                         class jl {
-                            constructor(e) {
-                                this.options = e, this.headings = [], this.headingRule = (e, t, n, r) => (1 === t ? this.currentTopHeading = this.saveHeading(e, t) : 2 === t && this.saveHeading(e, t, this.currentTopHeading && this.currentTopHeading.items, this.currentTopHeading && this.currentTopHeading.id), this.originalHeadingRule(e, t, n, r)), this.parser = new wl.Parser, this.headingEnhanceRenderer = new wl.Renderer, this.originalHeadingRule = this.headingEnhanceRenderer.heading.bind(this.headingEnhanceRenderer), this.headingEnhanceRenderer.heading = this.headingRule
+                            constructor(e, t) {
+                                this.options = e, this.parentId = t, this.headings = [], this.headingRule = (e, t, n, r) => (1 === t ? this.currentTopHeading = this.saveHeading(e, t) : 2 === t && this.saveHeading(e, t, this.currentTopHeading && this.currentTopHeading.items, this.currentTopHeading && this.currentTopHeading.id), this.originalHeadingRule(e, t, n, r)), this.parentId = t, this.parser = new wl.Parser, this.headingEnhanceRenderer = new wl.Renderer, this.originalHeadingRule = this.headingEnhanceRenderer.heading.bind(this.headingEnhanceRenderer), this.headingEnhanceRenderer.heading = this.headingRule
                             }
                             static containsComponent(e, t) {
                                 return new RegExp(Rl.replace(/{component}/g, t), "gmi").test(e)
                             }
                             static getTextBeforeHading(e, t) {
                                 const n = e.search(new RegExp(`^##?\\s+${t}`, "m"));
                                 return n > -1 ? e.substring(0, n) : e
                             }
                             saveHeading(e, t, n = this.headings, r) {
                                 e = e.replace(/&#(\d+);/g, ((e, t) => String.fromCharCode(parseInt(t, 10)))).replace(/&amp;/g, "&").replace(/&quot;/g, '"');
                                 const o = {
-                                    id: r ? `${r}/${no(e)}` : `section/${no(e)}`,
+                                    id: r ? `${r}/${no(e)}` : `${this.parentId||"section"}/${no(e)}`,
                                     name: e,
                                     level: t,
                                     items: []
                                 };
                                 return n.push(o), o
                             }
                             flattenHeadings(e) {
@@ -34187,15 +34187,15 @@
                                             title: r
                                         },
                                         refsStack: t
                                     };
                                     let o = this.byRef(e.$ref);
                                     if (!o) throw new Error(`Failed to resolve $ref "${e.$ref}"`);
                                     let i = t;
-                                    if (t.includes(e.$ref)) o = Object.assign({}, o, {
+                                    if (t.includes(e.$ref) || t.length > 999) o = Object.assign({}, o, {
                                         "x-circular-ref": !0
                                     });
                                     else if (this.isRef(o)) {
                                         const e = this.deref(o, t, n);
                                         i = e.refsStack, o = e.resolved
                                     }
                                     return i = pc(t, e.$ref), o = this.allowMergeRefs ? this.mergeRefs(e, o, n) : o, {
@@ -34234,33 +34234,39 @@
                                     }
                                 }
                                 return lc(lc({}, t), i)
                             }
                             mergeAllOf(e, t, n) {
                                 var r;
                                 if (e["x-circular-ref"]) return e;
-                                if (void 0 === (e = this.hoistOneOfs(e)).allOf) return e;
+                                if (void 0 === (e = this.hoistOneOfs(e, n)).allOf) return e;
                                 let o = cc(lc({}, e), {
                                     "x-parentRefs": [],
                                     allOf: void 0,
                                     title: e.title || ls(t)
                                 });
                                 void 0 !== o.properties && "object" == typeof o.properties && (o.properties = lc({}, o.properties)), void 0 !== o.items && "object" == typeof o.items && (o.items = lc({}, o.items));
-                                const i = e.allOf.map((e => {
+                                const i = function(e, t) {
+                                    const n = new Set;
+                                    return e.filter((e => {
+                                        const t = e.$ref;
+                                        return !t || t && !n.has(t) && n.add(t)
+                                    }))
+                                }(e.allOf.map((e => {
                                     var t;
                                     const {
                                         resolved: r,
                                         refsStack: i
                                     } = this.deref(e, n, !0), a = e.$ref || void 0, s = this.mergeAllOf(r, a, i);
                                     if (!s["x-circular-ref"] || !s.allOf) return a && (null == (t = o["x-parentRefs"]) || t.push(...s["x-parentRefs"] || [], a)), {
                                         $ref: a,
                                         refsStack: pc(i, a),
                                         schema: s
                                     }
-                                })).filter((e => void 0 !== e));
+                                })).filter((e => void 0 !== e)));
                                 for (const {
                                         schema: e,
                                         refsStack: n
                                     }
                                     of i) {
                                     const i = e,
                                         {
@@ -34281,15 +34287,17 @@
                                     if (o.type !== a && void 0 !== o.type && void 0 !== a && console.warn(`Incompatible types in allOf at "${t}": "${o.type}" and "${a}"`), void 0 !== a && (Array.isArray(a) && Array.isArray(o.type) ? o.type = [...a, ...o.type] : o.type = a), void 0 !== s && (Array.isArray(s) && Array.isArray(o.enum) ? o.enum = Array.from(new Set([...s, ...o.enum])) : o.enum = s), void 0 !== l && "object" == typeof l) {
                                         o.properties = o.properties || {};
                                         for (const e in l) {
                                             const i = dc(n, null == (r = l[e]) ? void 0 : r["x-refsStack"]);
                                             if (o.properties[e]) {
                                                 if (!y) {
                                                     const n = this.mergeAllOf({
-                                                        allOf: [o.properties[e], l[e]],
+                                                        allOf: [o.properties[e], cc(lc({}, l[e]), {
+                                                            "x-refsStack": i
+                                                        })],
                                                         "x-refsStack": i
                                                     }, t + "/properties/" + e, i);
                                                     o.properties[e] = n
                                                 }
                                             } else o.properties[e] = cc(lc({}, l[e]), {
                                                 "x-refsStack": i
                                             })
@@ -34319,25 +34327,26 @@
                                     const {
                                         resolved: o
                                     } = this.deref(n[r]);
                                     void 0 !== o.allOf && o.allOf.find((t => void 0 !== t.$ref && e.indexOf(t.$ref) > -1)) && (t["#/components/schemas/" + r] = [o["x-discriminator-value"] || r])
                                 }
                                 return t
                             }
-                            hoistOneOfs(e) {
+                            hoistOneOfs(e, t) {
                                 if (void 0 === e.allOf) return e;
-                                const t = e.allOf;
-                                for (let e = 0; e < t.length; e++) {
-                                    const n = t[e];
-                                    if (Array.isArray(n.oneOf)) {
-                                        const r = t.slice(0, e),
-                                            o = t.slice(e + 1);
+                                const n = e.allOf;
+                                for (let e = 0; e < n.length; e++) {
+                                    const r = n[e];
+                                    if (Array.isArray(r.oneOf)) {
+                                        const o = n.slice(0, e),
+                                            i = n.slice(e + 1);
                                         return {
-                                            oneOf: n.oneOf.map((e => ({
-                                                allOf: [...r, e, ...o]
+                                            oneOf: r.oneOf.map((e => ({
+                                                allOf: [...o, e, ...i],
+                                                "x-refsStack": t
                                             })))
                                         }
                                     }
                                 }
                                 return e
                             }
                         }
@@ -34411,15 +34420,16 @@
                                             refsStack: o
                                         } = t.deref(e, this.refsStack, !0), i = t.mergeAllOf(r, this.pointer + "/oneOf/" + n, o), a = ss(e.$ref) && !i.title ? Da.baseName(e.$ref) : `${i.title||""}${i.const&&JSON.stringify(i.const)||""}`;
                                         return new Sc(t, _c(kc({}, i), {
                                             title: a,
                                             allOf: [_c(kc({}, this.schema), {
                                                 oneOf: void 0,
                                                 anyOf: void 0
-                                            })]
+                                            })],
+                                            discriminator: r.allOf ? void 0 : i.discriminator
                                         }), e.$ref || this.pointer + "/oneOf/" + n, this.options, !1, o)
                                     })), this.options.simpleOneOfTypeLabel) {
                                     const e = function(e) {
                                         const t = new Set;
                                         return function e(n) {
                                             for (const r of n.oneOf || []) r.oneOf ? e(r) : r.type && t.add(r.type)
                                         }(e), Array.from(t.values())
@@ -37347,15 +37357,15 @@
                             static buildStructure(e, t) {
                                 const n = e.spec,
                                     r = [],
                                     o = df.getTagsWithOperations(e, n);
                                 return r.push(...df.addMarkdownItems(n.info.description || "", void 0, 1, t)), n["x-tagGroups"] && n["x-tagGroups"].length > 0 ? r.push(...df.getTagGroupsItems(e, void 0, n["x-tagGroups"], o, t)) : r.push(...df.getTagsItems(e, o, void 0, void 0, t)), r
                             }
                             static addMarkdownItems(e, t, n, r) {
-                                const o = new jl(r).extractHeadings(e || "");
+                                const o = new jl(r, null == t ? void 0 : t.id).extractHeadings(e || "");
                                 o.length && t && t.description && (t.description = jl.getTextBeforeHading(t.description, o[0].name));
                                 const i = (e, t, n = 1) => t.map((t => {
                                     const r = new tf("section", t, e);
                                     return r.depth = n, t.items && (r.items = i(r, t.items, n + 1)), r
                                 }));
                                 return i(t, o, n)
                             }
@@ -37584,15 +37594,15 @@
                                     } else e = r(4798).default;
                                     return new e
                                 }()
                             }
                             indexItems(e) {
                                 const t = e => {
                                     e.forEach((e => {
-                                        "group" !== e.type && this.add(e.name, e.description || "", e.id), t(e.items)
+                                        "group" !== e.type && this.add(e.name, (e.description || "").concat(" ", e.path || ""), e.id), t(e.items)
                                     }))
                                 };
                                 t(e), this.searchWorker.done()
                             }
                             add(e, t, n) {
                                 this.searchWorker.add(e, t, n)
                             }
@@ -39992,15 +40002,15 @@
                 }
                 renderWithOptionsAndStore(e, t) {
                     const {
                         source: r,
                         htmlWrap: o = (e => e)
                     } = this.props;
                     if (!t) throw new Error("When using components in markdown, store prop must be provided");
-                    const i = new jl(e).renderMdWithComponents(r);
+                    const i = new jl(e, this.props.parentId).renderMdWithComponents(r);
                     return i.length ? i.map(((e, r) => {
                         if ("string" == typeof e) return n.cloneElement(o(n.createElement(Mf, {
                             html: e,
                             inline: !1,
                             compact: !1
                         })), {
                             key: r
@@ -40081,14 +40091,18 @@
             }, n) {
                 return e > 1 ? t.sidebar.level1Items[n] : 1 === e ? t.sidebar.groupItems[n] : ""
             }
             const _y = ga.ul`
   margin: 0;
   padding: 0;
 
+  &:first-child {
+    padding-bottom: 32px;
+  }
+
   & & {
     font-size: 0.929em;
   }
 
   ${e=>e.expanded?"":"display: none;"};
 `,
                 Oy = ga.li`
@@ -40147,48 +40161,49 @@
   display: inline-block;
   vertical-align: middle;
   width: ${e=>e.width?e.width:"auto"};
   overflow: hidden;
   text-overflow: ellipsis;
 `,
                 Ay = ga.div`
-  ${({theme:e})=>`\
-            n font - size: 0.8 em;\
-            n margin - top: $ {
+  ${({theme:e})=>pa`
+            font - size: 0.8 em;
+            margin - top: $ {
                 2 * e.spacing.unit
             }
-            px;\
-            n text - align: center;\
-            n position: fixed;\
-            n width: $ {
+            px;
+            text - align: center;
+            position: fixed;
+            width: $ {
                 e.sidebar.width
-            };\
-            n bottom: 0 px;\
-            n background: $ {
+            };
+            bottom: 0;
+            background: $ {
                 e.sidebar.backgroundColor
-            };\
-            n\ n a, \n a: visited, \n a: hover {
-                \
-                n color: $ {
-                    e.sidebar.textColor
-                }!important;\
-                n padding: $ {
-                    e.spacing.unit
+            };
+
+            a,
+            a: visited,
+                a: hover {
+                    color: $ {
+                        e.sidebar.textColor
+                    }!important;
+                    padding: $ {
+                        e.spacing.unit
+                    }
+                    px 0;
+                    border - top: 1 px solid $ {
+                        Rr(.1, e.sidebar.backgroundColor)
+                    };
+                    text - decoration: none;
+                    display: flex;
+                    align - items: center;
+                    justify - content: center;
                 }
-                px 0;\
-                n border - top: 1 px solid $ {
-                    Rr(.1, e.sidebar.backgroundColor)
-                };\
-                n text - decoration: none;\
-                n display: flex;\
-                n align - items: center;\
-                n justify - content: center;\
-                n
-            }\
-            n`};
+            `};
   img {
     width: 15px;
     margin-right: 5px;
   }
 
   ${ma("small")`
     width: 100%;
@@ -40684,15 +40699,17 @@
 
             function hv(e) {
                 const {
                     security: t,
                     showSecuritySchemeType: r,
                     expanded: o
                 } = e, i = t.schemes.length > 1;
-                return n.createElement(Fg, {
+                return 0 === t.schemes.length ? n.createElement(Fg, {
+                    expanded: o
+                }, "None") : n.createElement(Fg, {
                     expanded: o
                 }, i && "(", t.schemes.map((e => n.createElement(Mg, {
                     key: e.id
                 }, r && `${Jg[e.type]||e.type}: `, n.createElement("i", null, e.displayName), o && e.scopes.length ? [" (", e.scopes.map((e => n.createElement(Lg, {
                     key: e
                 }, e))), ") "] : null))), i && ") ")
             }
@@ -41187,14 +41204,15 @@
                         level: o
                     } = this.props.item, i = 2 === o ? ju : Ru;
                     return n.createElement(n.Fragment, null, n.createElement(Au, null, n.createElement(Ou, {
                         compact: !1
                     }, n.createElement(i, null, n.createElement(Uu, {
                         to: this.props.item.id
                     }), e))), n.createElement(vy, {
+                        parentId: this.props.item.id,
                         source: t || "",
                         htmlWrap: ub
                     }), r && n.createElement(Au, null, n.createElement(Ou, null, n.createElement(xm, {
                         externalDocs: r
                     }))))
                 }
             };
@@ -41855,16 +41873,16 @@
                     if (Jb)
                         for (var n of Jb(t)) ew.call(t, n) && tw(e, n, t[n]);
                     return e
                 };
             Nt({
                 useProxies: "ifavailable"
             });
-            const rw = "2.0.0-rc.75",
-                ow = "d7440fb";
+            const rw = "2.0.0",
+                ow = "5fb4daa";
 
             function iw(e) {
                 const t = function(e) {
                         const t = {},
                             n = e.attributes;
                         for (let e = 0; e < n.length; e++) {
                             const r = n[e];
```

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   Licensed under the MIT License (MIT), see
   http://jedwatson.github.io/classnames
 */
 
 /*!
  * ReDoc - OpenAPI/Swagger-generated API Reference Documentation
  * -------------------------------------------------------------
- *   Version: "2.0.0-rc.75"
+ *   Version: "2.0.0"
  *   Repo: https://github.com/Redocly/redoc
  */
 
 /*!
  * Stickyfill -- `position: sticky` polyfill
  * v. 1.1.1 | https://github.com/wilddeer/stickyfill
  * Copyright Oleg Korsunsky | http://wd.dizaina.net/
```

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/LICENSE` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/static/swagger/swagger-ui.css` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/static/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.0.1/fastapi_standalone_docs/tests/test_standalone_docs.py` & `fastapi_standalone_docs-0.1.0/fastapi_standalone_docs/tests/test_standalone_docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,24 +78,22 @@
 
 
 def test_swagger_disabled():
     app = FastAPI(docs_url=None)
     StandaloneDocs(app)
     client = TestClient(app)
 
-    response = client.get("/docs")
-    assert response.status_code == 404
-
-    resources = (
+    paths = (
+        "/docs",
         "/docs/swagger-ui.css",
         "/docs/fastapi/favicon.png",
         "/docs/swagger-ui-bundle.js",
     )
-    for res in resources:
-        response = client.get(res)
+    for path in paths:
+        response = client.get(path)
         assert response.status_code == 404
 
 
 def test_redoc_default():
     app = FastAPI()
     StandaloneDocs(app)
     client = TestClient(app)
@@ -167,28 +165,46 @@
 
 
 def test_redoc_disabled():
     app = FastAPI(redoc_url=None)
     StandaloneDocs(app)
     client = TestClient(app)
 
-    response = client.get("/redoc")
-    assert response.status_code == 404
-
-    resources = (
-        "/my-redoc-url/logo-mini.svg",
-        "/my-redoc-url/redoc.standalone.js",
-        "/my-redoc-url/fastapi/favicon.png",
+    paths = (
+        "/redoc",
+        "/redoc/logo-mini.svg",
+        "/redoc/redoc.standalone.js",
+        "/redoc/fastapi/favicon.png",
     )
-    for res in resources:
-        response = client.get(res)
+    for path in paths:
+        response = client.get(path)
         assert response.status_code == 404
 
 
 def test_redoc_with_google_fonts():
     app = FastAPI()
     StandaloneDocs(app, with_google_fonts=True)
     client = TestClient(app)
 
     response = client.get("/redoc")
     assert response.status_code == 200
     assert "https://fonts.googleapis.com" in response.text
+
+
+def test_openapi_disabled():
+    app = FastAPI(openapi_url=None)
+    StandaloneDocs(app)
+    client = TestClient(app)
+
+    paths = (
+        "/docs",
+        "/docs/swagger-ui.css",
+        "/docs/fastapi/favicon.png",
+        "/docs/swagger-ui-bundle.js",
+        "/redoc",
+        "/redoc/logo-mini.svg",
+        "/redoc/redoc.standalone.js",
+        "/redoc/fastapi/favicon.png",
+    )
+    for path in paths:
+        response = client.get(path)
+        assert response.status_code == 404
```

### Comparing `fastapi_standalone_docs-0.0.1/pyproject.toml` & `fastapi_standalone_docs-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-standalone-docs"
-version = "0.0.1"
+version = "0.1.0"
 description = "Host FastAPI Swagger UI and ReDoc without third party CDNs"
 authors = ["IOXIO Ltd"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "fastapi_standalone_docs"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fastapi_standalone_docs-0.0.1/PKG-INFO` & `fastapi_standalone_docs-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-standalone-docs
-Version: 0.0.1
+Version: 0.1.0
 Summary: Host FastAPI Swagger UI and ReDoc without third party CDNs
 License: MIT
 Author: IOXIO Ltd
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -94,14 +94,22 @@
 app = FastAPI()
 StandaloneDocs(
     app=app,
     with_google_fonts=True,
 )
 ```
 
+### Disclaimer
+
+**Note!** If you create multiple FastAPI apps in the same runtime (quite unlikely
+use-case), using StandaloneDocs on one of them will affect the other ones as well, as
+the library patches two of the shared functions (`get_swagger_ui_html` and
+`get_redoc_html`). Thus the library should not be used in a such setup unless all the
+apps will use StandaloneDocs with the same settings.
+
 ## Development
 
 PRs are welcome!
 
 This project is using [Poetry](https://python-poetry.org/) and
 [pre-commit](https://pre-commit.com/), so please ensure you've installed both. To set up
 the project with them run:
```

