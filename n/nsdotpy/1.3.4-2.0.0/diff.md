# Comparing `tmp/nsdotpy-1.3.4.tar.gz` & `tmp/nsdotpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.3.4.tar", max compression
+gzip compressed data, was "nsdotpy-2.0.0.tar", max compression
```

## Comparing `nsdotpy-1.3.4.tar` & `nsdotpy-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-22 08:06:54.591861 nsdotpy-1.3.4/LICENSE.md
--rw-r--r--   0        0        0     2440 2023-05-22 08:06:54.591861 nsdotpy-1.3.4/README.md
--rw-r--r--   0        0        0      790 2023-05-22 08:06:54.607861 nsdotpy-1.3.4/nsdotpy/__init__.py
--rw-r--r--   0        0        0    46894 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/nsdotpy/valid.py
--rw-r--r--   0        0        0      719 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-06-20 03:08:11.893972 nsdotpy-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2847 2023-06-20 03:08:11.893972 nsdotpy-2.0.0/README.md
+-rw-r--r--   0        0        0      787 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    49237 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/session.py
+-rw-r--r--   0        0        0     5033 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/valid.py
+-rw-r--r--   0        0        0      786 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 nsdotpy-2.0.0/PKG-INFO
```

### Comparing `nsdotpy-1.3.4/LICENSE.md` & `nsdotpy-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.4/README.md` & `nsdotpy-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 ```python
 
 from nsdotpy.session import NSSession
 session = NSSession("NSDotPy Example", "1.0.0", "Script Author's nation", "Script User's nation")
 
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
+
+# an API client is also available, here's a simple example
+data = session.api_request("world", shard="nations")
+# it returns a benedict object (https://github.com/fabiocaccamo/python-benedict), which is a dict with some extra features
+# you can access the data like a normal dict
+nations = data["nations"].split(",")
+# or you can use a keyattribute (my personal favorite)
+nations = data.nations.split(",")
 ```
 
 ## TODO:
 
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
```

### Comparing `nsdotpy-1.3.4/nsdotpy/__init__.py` & `nsdotpy-2.0.0/nsdotpy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of NSDotPy, a wrapper around requests that makes interacting
+# This file is part of NSDotPy, a wrapper around httpx that makes interacting
 # with the HTML nationstates.net site legally and efficiently easier.
 #
 # NSDotPy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation either version
 # 3 of the License, or (at your option) any later version.
 #
```

### Comparing `nsdotpy-1.3.4/nsdotpy/session.py` & `nsdotpy-2.0.0/nsdotpy/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import mimetypes  # for flag and banner uploading
 
 # external library imports
 import keyboard  # for the required user input
 import httpx  # for http stuff
 from tendo.singleton import SingleInstance  # so it can only be run once at a time
 from bs4 import BeautifulSoup, Tag  # for parsing html and xml
+from benedict import benedict
 
 # local imports
 from . import valid  # for valid region tags
 
 
 def canonicalize(string: str) -> str:
     """Converts a string to its canonical form used by the nationstates api.
@@ -62,50 +63,75 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.3.4"
+        self.VERSION = "2.0.0"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
         self._me = SingleInstance()
         # Create a new httpx session
-        self._session = httpx.Client(http2=True, timeout=30)  # ns can b slow
+        self._session = httpx.Client(
+            http2=True, timeout=30
+        )  # ns can b slow, 30 seconds is hopefully a good sweet spot
         # Set the user agent to the script name, version, author, and user as recommended in the script rules thread:
         # https://forum.nationstates.net/viewtopic.php?p=16394966&sid=be37623536dbc8cee42d8d043945b887#p16394966
         self._lock: bool = False
         self._set_user_agent(
             script_name, script_version, script_author, script_user, link_to_src
         )
-        # If a link to the source code is provided, add it to the user agent
-        self._ns_server = "1"
         # Initialize nationstates specific stuff
         self._auth_region = "rwby"
         self.chk: str = ""
         self.localid: str = ""
         self.pin: str = ""
         self.nation: str = ""
         self.region: str = ""
-        self.api_pin: str = ""
-        self.current_page: tuple[str, str] = ("", "")
         self.keybind = keybind
         # Make sure the nations in the user agent actually exist
-        if not self._validate_nations([script_author, script_user]):
+        if not self._validate_nations({script_author, script_user}):
             raise ValueError(
                 "One of, or both, of the nations in the user agent do not exist. Make sure you're only including the nation name in the constructor, e.g. 'Thorn1000' instead of 'Devved by Thorn1000'"
             )
         self.logger.info(f"Initialized. Keybind to continue is {self.keybind}.")
 
+    def _validate_shards(self, api: str, shards: set[str]) -> None:
+        """Makes sure a given payload to the nationstates API is valid.
+
+        Args:
+            API (str): The API to validate the payload for
+            Shard (set): The shards to validate the payload for
+        """
+        for shard in shards:
+            match api:
+                case "nation":
+                    if (
+                        shard
+                        not in valid.NATION_SHARDS
+                        | valid.PRIVATE_NATION_SHARDS
+                        | valid.PRIVATE_NATION_SHARDS
+                    ):
+                        raise ValueError(f"{shard} is not a valid shard for {api}")
+                case "region":
+                    if shard not in valid.REGION_SHARDS:
+                        raise ValueError(f"{shard} is not a valid shard for {api}")
+                case "world":
+                    if shard not in valid.WORLD_SHARDS:
+                        raise ValueError(f"{shard} is not a valid shard for {api}")
+                case "wa":
+                    if shard not in valid.WA_SHARDS:
+                        raise ValueError(f"{shard} is not a valid shard for {api}")
+
     def _set_user_agent(
         self,
         script_name: str,
         script_version: str,
         script_author: str,
         script_user: str,
         link_to_src: str,
@@ -114,31 +140,25 @@
             f"{script_name}/{script_version} (by:{script_author}; usedBy:{script_user})"
         )
         if link_to_src:
             self.user_agent = f"{self.user_agent}; src:{link_to_src}"
         self.user_agent = f"{self.user_agent}; Written with NSDotPy/{self.VERSION} (by:Sweeze; src:github.com/sw33ze/NSDotPy)"
         self._session.headers.update({"User-Agent": self.user_agent})
 
-    def _validate_nations(self, nations: list[str]) -> bool:
+    def _validate_nations(self, nations: set[str]) -> bool:
         """Checks if a list of nations exist using the NationStates API.
 
         Args:
-            nations (list[str]): List of nations to check
+            nations (set[str]): List of nations to check
 
         Returns:
-            bool: True if all nations in the list exist, False otherwise.
+            bool: True if all nations in the set exist, False otherwise.
         """
-        url = "https://www.nationstates.net/cgi-bin/api.cgi"
-        data = {"q": "nations"}
-        response = self.request(url, data)
-        soup = BeautifulSoup(response.text, "lxml-xml")
-        # the list of nations is inside the <NATIONS> tag
-        world_nations_tag: Tag = soup.find("NATIONS")  # type: ignore
-        # get the list of nations from the <NATIONS> tag
-        world_nations: list[str] = world_nations_tag.text.split(",")
+        response = self.api_request("world", shard="nations")
+        world_nations = response.nations.split(",")
         # check if all nations in the list exist in the world nations
         return all(canonicalize(nation) in world_nations for nation in nations)
 
     def _init_logger(self):
         self.logger = logging.getLogger("NSDotPy")
         config = {
             "version": 1,
@@ -171,28 +191,21 @@
         # gathering chk and localid so i dont have to worry about authenticating l8r
         if chk := soup.find("input", {"name": "chk"}):
             self.chk = chk["value"].strip()  # type: ignore
         if localid := soup.find("input", {"name": "localid"}):
             self.localid = localid["value"].strip()  # type: ignore
         if pin := self._session.cookies.get("pin"):
             # you should never really need the pin but just in case i'll store it
+            # PAST ME WAS RIGHT, I NEEDED IT FOR THE PRIVATE API!!
             self.pin = pin
         if soup.find("a", {"class": "STANDOUT"}):
             self.region = canonicalize(
                 soup.find_all("a", {"class": "STANDOUT"})[1].attrs["href"].split("=")[1]
             )
 
-    def _refresh_auth_values(self):
-        self.logger.info("Refreshing authentication values...")
-        response = self.request(
-            f"https://www.nationstates.net/page=display_region/region={self._auth_region}",
-            data={"theme": "century"},
-        )
-        self._get_auth_values(response)
-
     def _wait_for_input(self, key: str) -> int:
         """Blocks execution until the user presses a key. Used as the one click = one request action.
 
         Args:
             key (str): The key to wait for
 
         Returns:
@@ -205,15 +218,15 @@
         return int(time.time() * 1000)
 
     def _get_detag_wfe(self) -> str:
         """Gets the detagged WFE of the region you're in.
 
         Returns:
             str: The detagged WFE"""
-        self.logger.info(f"Getting detagged WFE for {self.region}...")
+        self.logger.info(f"Getting detag WFE for {self.region}...")
         response = self.request(
             f"https://greywardens.xyz/tools/wfe_index/region={self.region}",
         )
         soup = BeautifulSoup(response.text, "lxml")
         # the safest bet for a detag wfe is the first wfe of the region
         return soup.find_all("pre")[-1].text
 
@@ -239,55 +252,43 @@
             # check if pretitle contains any non-alphanumeric characters (except spaces)
             if key == "pretitle" and not value.replace(" ", "").isalnum():
                 raise ValueError(
                     "Pretitle should only contain alphanumeric characters or spaces."
                 )
 
     def _html_request(
-        self, url, data={}, files=None, follow_redirects=False, auth=()
+        self, url, data={}, files=None, follow_redirects=False
     ) -> httpx.Response:
         data |= {"chk": self.chk, "localid": self.localid}
         userclick = self._wait_for_input(self.keybind)
         # userclick is the number of milliseconds since the epoch, admin uses this for help enforcing the simultaneity rule
         response = self._session.post(
             f"{url}/userclick={userclick}",
             data=data,
             files=files,
             follow_redirects=follow_redirects,
-            auth=auth,
         )
         if response.status_code >= 400:
             with open("error.html", "w") as f:
                 f.write(response.text)
             raise httpx.HTTPError(
                 f"Received status code {response.status_code} from {response.url}. Error page saved to error.html."
             )
         self._get_auth_values(response)
         return response
 
     # --- end private methods --- #
 
-    def NS2_authenticate(self, user: str, password: str):
-        """Authenticates the user to nationstates2.net with the given credentials.
-
-        Args:
-            user (str): The username supplied
-            password (str): The password supplied
-
-        Returns:
-            bool: True if the authentication was successful, False otherwise"""
-        url = "https://www.nationstates2.net/template-overall=none/"
-        self._auth_user = user
-        self._auth_password = password
-        response = self._html_request(url, auth=(user, password))
-        if response.status_code == 200:
-            self._ns_server = "2"
-            self._auth_region = "the_black_hawks"
-            return True
-        return False
+    def refresh_auth_values(self):
+        self.logger.info("Refreshing authentication values...")
+        response = self.request(
+            f"https://www.nationstates.net/page=display_region/region={self._auth_region}",
+            data={"theme": "century"},
+        )
+        self._get_auth_values(response)
 
     def request(
         self,
         url: str,
         data: dict = {},
         files: dict = {},
         follow_redirects: bool = False,
@@ -298,93 +299,116 @@
             url (str): URL to send the request to
             data (dict, optional): Payload to send with the request
             files (dict, optional): Payload to send with requests that upload files
 
         Returns:
             httpx.Response: The response from the server
         """
-        auth = None
-        if self._ns_server != "1":
-            url = url.replace("nationstates.net", f"nationstates{self._ns_server}.net")
-            auth = (self._auth_user, self._auth_password)
         if any(
             banned_page in canonicalize(url)
-            for banned_page in [
+            for banned_page in {
                 "page=telegrams",
                 "page=dilemmas",
                 "page=compose_telegram",
                 "page=store",
-            ]
+                "page=help",
+            }
         ):
             raise ValueError(
                 "You cannot use a tool to interact with telegrams, issues, getting help, or the store. Read up on the script rules: https://forum.nationstates.net/viewtopic.php?p=16394966#p16394966"
             )
         if self._lock:
             # if lock is true then we're already in the middle of a
             # request and we're in danger of breaking the simultaneity rule
             # so raise an error
             raise PermissionError(
                 "You're already in the middle of a request. Stop trying to violate simultaneity."
             )
         self._lock = True
         if "api.cgi" in canonicalize(url):
-            # deal with ratelimiting if its an api request
-            response = self.api_request(data, _auth=auth)
+            # you should be using api_request for api requests
+            raise ValueError("You should be using api_request() for api requests.")
         elif "nationstates" in canonicalize(url):
             # do all the things that need to be done for html requests
-            response = self._html_request(url, data, files, follow_redirects, auth=auth)
+            response = self._html_request(url, data, files, follow_redirects)
         else:
             # if its not nationstates then just pass the request through
             response = self._session.post(
                 url, data=data, follow_redirects=follow_redirects
             )
-        self.current_page = (url, response.text)
         self._lock = False
         return response
 
-    def api_request(self, data: dict, password: str = "", _auth=()) -> httpx.Response:
+    def api_request(
+        self,
+        api: str,
+        *,
+        target: str = "",
+        shard: str | set[str] = "",
+        password: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
         """Sends a request to the nationstates api with the given data.
 
         Args:
-            data (dict): Payload to send with the request, e.g. {"nation": "testlandia", "q": "region"}
-            password (str, optional): The password to use for authenticating private api requests. Defaults to "".
-            _auth (tuple, optional): The username and password to use for authentication to an alternative nationstates server. Defaults to ().
+            api (str): The api to send the request to. Must be "nation", "region", "world", or "wa"
+            target (str, optional): The nation, region, or wa council to target. Required for non-world api requests.
+            shard (str, optional): The shard, or shards, you're requesting for. Must be a valid shard for the given api. Only required for world and wa api requests.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
 
         Returns:
-            httpx.Response: The response from the server
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
         """
         # TODO: probably move this responsibility to a third party api library to avoid reinventing the wheel
         # if one exists of sufficient quality thats AGPLv3 compatible
-        data |= {"v": "12"}
-        url = (
-            f"https://www.nationstates{self._ns_server}.net/cgi-bin/api.cgi"
-            if _auth
-            else "https://www.nationstates.net/cgi-bin/api.cgi"
-        )
+        if api not in {"nation", "region", "world", "wa"}:
+            raise ValueError("api must be 'nation', 'region', 'world', or 'wa'")
+        if api != "world" and not target:
+            raise ValueError("target must be specified for non-world api requests")
+        if api in {"wa", "world"} and not shard:
+            raise ValueError("shard must be specified for world and wa api requests")
+        # end argument validation
+        # shard validation
+        if type(shard) == str:
+            shard = {shard}
+        self._validate_shards(api, shard)  # type: ignore
+        # end shard validation
+        data = {
+            "v": "12",
+        }
+        if api != "world":
+            data[api] = target
+        if shard:
+            data["q"] = "+".join(shard)
+        url = "https://www.nationstates.net/cgi-bin/api.cgi"
         if password:
             self._session.headers["X-Password"] = password
-        if self.api_pin:
-            self._session.headers["X-Pin"] = self.api_pin
+        if self.pin:
+            self._session.headers["X-Pin"] = self.pin
         # rate limiting section
-        response = self._session.post(url, data=data, auth=_auth)
+        response = self._session.post(url, data=data)
         # if the server tells us to wait, wait
         head = response.headers
         if "X-Pin" in head:
-            self.api_pin = head["X-Pin"]
+            self.pin = head["X-Pin"]
         if waiting_time := head.get("Retry-After"):
             self.logger.warning(f"Rate limited. Waiting {waiting_time} seconds.")
             time.sleep(int(waiting_time))
         # slow down requests so we dont hit the rate limit in the first place
         requests_left = int(head["RateLimit-Remaining"])
-        seconds_until_reset = int(head["RateLimit-Reset"])
-        # only slow down if we're close to the limit to avoid slowing down one off or infrequent requests
-        if requests_left < 10:
+        if requests_left < 10 or constant_rate_limit:
+            seconds_until_reset = int(head["RateLimit-Reset"])
             time.sleep(seconds_until_reset / requests_left)
         # end rate limiting section
-        return response
+        response.raise_for_status()
+        parsed_response = benedict.from_xml(response.text, keyattr_dynamic=True)
+        parsed_response.standardize()
+        parsed_response: benedict = parsed_response[api]  # type: ignore
+        return parsed_response
 
     def login(self, nation: str, password: str) -> bool:
         """Logs in to the nationstates site.
 
         Args:
             nation (str): Nation name
             password (str): Nation password
@@ -437,15 +461,15 @@
                 mimetypes.guess_type(flag_filename)[0],
             )
         }
 
         response = self.request(url, data=data, files=files)
 
         if "page=settings" in response.headers["location"]:
-            self._refresh_auth_values()
+            self.refresh_auth_values()
             return True
         elif "Just a moment..." in response.text:
             self.logger.warning(
                 "Cloudflare blocked you idiot get fucked have fun with that like I had to lmaoooooooooo"
             )
         return False
 
@@ -560,15 +584,15 @@
         url = "https://www.nationstates.net/cgi-bin/join_un.cgi"
 
         data = {"nation": canonicalize(nation), "appid": app_id.strip()}
         response = self.request(url, data)
 
         if "?welcome=1" in response.headers["location"]:
             # since we're just getting thrown into a cgi script, we'll have to manually grab authentication values
-            self._refresh_auth_values()
+            self.refresh_auth_values()
             return True
         return False
 
     def resign_wa(self):
         """Resigns from the WA.
 
         Returns:
@@ -639,36 +663,40 @@
         self.logger.info(f"Clearing dossier on {self.nation}")
         url = "https://www.nationstates.net/template-overall=none/page=dossier"
         data = {"clear_dossier": "1"}
         response = self.request(url, data)
 
         return "Dossier cleared of nations." in response.text
 
-    def add_to_dossier(self, nations: list[str]) -> bool:
+    def add_to_dossier(self, nations: list[str] | str) -> bool:
         """Adds nations to the logged in nation's dossier.
 
         Args:
-            nations (list[str]): List of nations to add
+            nations (list[str] | str): List of nations to add, or a single nation
 
         Returns:
             bool: Whether it was successful or not
         """
 
         self.logger.info(f"Adding {nations} to dossier on {self.nation}")
         url = "https://www.nationstates.net/dossier.cgi"
         data = {
             "currentnation": canonicalize(self.nation),
             "action_append": "Upload Nation Dossier File",
         }
         files = {
-            "file": ("dossier.txt", "\n".join(nations), "text/plain"),
+            "file": (
+                "dossier.txt",
+                "\n".join(nations).strip() if type(nations) is list else nations,
+                "text/plain",
+            ),
         }
         response = self.request(url, data, files=files)
 
-        self._refresh_auth_values()
+        self.refresh_auth_values()
         return "appended=" in response.headers["location"]
 
     def wa_vote(self, council: str, vote: str) -> bool:
         """Votes on the current WA resolution.
 
         Args:
             council (str): Must be "ga" for general assembly, "sc" for security council.
@@ -676,17 +704,17 @@
 
         Returns:
             bool: Whether the vote was successful or not
         """
         self.logger.info(
             f"Voting {vote} on {council.upper()} resolution with {self.nation}"
         )
-        if council not in ["ga", "sc"]:
+        if council not in {"ga", "sc"}:
             raise ValueError("council must be 'ga' or 'sc'")
-        if vote not in ["for", "against"]:
+        if vote not in {"for", "against"}:
             raise ValueError("vote must be 'for' or 'against'")
         self.logger.info("Voting on WA resolution")
 
         url = f"https://www.nationstates.net/template-overall=none/page={council}"
         data = {
             "vote": f"Vote {vote.capitalize()}",
         }
@@ -733,17 +761,42 @@
         }
         self._validate_fields(data)
 
         response = self.request(url, data)
 
         if "?founded=new" not in response.headers["location"]:
             return False
-        self._refresh_auth_values()
+        self.nation = nation_name
+        self.refresh_auth_values()
         return True
 
+    def refound_nation(self, nation: str, password: str) -> bool:
+        """Refounds a nation.
+
+        Args:
+            nation (str): Name of the nation to refound
+            password (str): Password to the nation
+
+        Returns:
+            bool: Whether the nation was successfully refounded or not
+        """
+        url = "https://www.nationstates.net/template-overall=none/"
+        data = {
+            "logging_in": "1",
+            "restore_password": password,
+            "restore_nation": "1",
+            "nation": nation,
+        }
+        response = self.request(url, data=data)
+        if response.status_code == 302:
+            self.nation = nation
+            self.refresh_auth_values()
+            return True
+        return False
+
     # methods for region control
 
     def create_region(
         self,
         region_name: str,
         wfe: str,
         *,
@@ -763,16 +816,16 @@
         Returns:
             bool: Whether the region was successfully created or not
         """
         self.logger.info(f"Creating new region {region_name}")
         url = "https://www.nationstates.net/template-overall=none/page=create_region"
         data = {
             "page": "create_region",
-            "region_name": region_name,
-            "desc": wfe,
+            "region_name": region_name.strip(),
+            "desc": wfe.strip(),
             "create_region": "1",
         }
         if password:
             data |= {"pw": "1", "rpassword": password}
         if frontier:
             data |= {"is_frontier": "1"}
         elif executive_delegacy:
@@ -790,15 +843,15 @@
         Raises:
             ValueError: If type is not "flag" or "banner"
 
         Returns:
             str: Empty string if the upload failed, otherwise the ID of the uploaded file
         """
         self.logger.info(f"Uploading {filename} to {self.region}")
-        if type not in ["flag", "banner"]:
+        if type not in {"flag", "banner"}:
             raise ValueError("type must be 'flag' or 'banner'")
         url = "https://www.nationstates.net/cgi-bin/upload.cgi"
         data = {
             "uploadtype": f"r{type}",
             "page": "region_control",
             "region": self.region,
             "expect": "json",
@@ -825,15 +878,15 @@
 
         Raises:
             ValueError: If flagmode is not "flag", "logo", or ""
 
         Returns:
             bool: Whether the change was successful or not
         """
-        if flag_mode not in ["flag", "logo", ""]:
+        if flag_mode not in {"flag", "logo", ""}:
             raise ValueError("flagmode must be 'flag', 'logo', or ''")
         self.logger.info(f"Setting flag and banner for {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             "newflag": flag_id,
             "newbanner": banner_id,
             "saveflagandbannerchanges": "1",
@@ -944,44 +997,44 @@
 
         Raises:
             ValueError: If action is not "add" or "remove", or if tag is not a valid tag.
 
         Returns:
             bool: Whether the tag was successfully added or removed
         """
-        if action not in ["add", "remove"]:
+        if action not in {"add", "remove"}:
             raise ValueError("action must be 'add' or 'remove'")
-        if canonicalize(tag) not in valid.region_tags:
+        if canonicalize(tag) not in valid.REGION_TAGS:
             raise ValueError(f"{tag} is not a valid tag")
         self.logger.info(f"{action.capitalize()}ing tag {tag} for {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             f"{action}_tag": canonicalize(tag),
             "updatetagsbutton": "1",
         }
         response = self.request(url, data)
         return "Region Tags updated!" in response.text
 
     def eject(self, nation: str) -> bool:
-        """Ejects a nation from the current region.
+        """Ejects a nation from the current region. Note that a 1 second delay is required before ejecting another nation.
 
         Args:
             nation (str): The nation to eject.
 
         Returns:
             bool: Whether the nation was successfully ejected or not
         """
         self.logger.info(f"Ejecting {nation} from {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {"nation_name": nation, "eject": "1"}
         response = self.request(url, data)
         return "has been ejected from " in response.text
 
     def banject(self, nation: str) -> bool:
-        """Bans a nation from the current region.
+        """Bans a nation from the current region. Note that a 1 second delay is required before banjecting another nation.
 
         Args:
             nation (str): The nation to banject.
 
         Returns:
             bool: Whether the nation was successfully banjected or not
         """
```

### Comparing `nsdotpy-1.3.4/nsdotpy/valid.py` & `nsdotpy-2.0.0/nsdotpy/valid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of NSDotPy, a wrapper around requests that makes interacting
+# This file is part of NSDotPy, a wrapper around httpx that makes interacting
 # with the HTML nationstates.net site legally and efficiently easier.
 #
 # NSDotPy is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License
 # as published by the Free Software Foundation either version
 # 3 of the License, or (at your option) any later version.
 #
@@ -10,15 +10,15 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with NSDotPy. If not, see <https://www.gnu.org/licenses/>.
 
-region_tags: list[str] = [
+REGION_TAGS: set[str] = {
     "anarchist",
     "anime",
     "anti-capitalist",
     "anti-communist",
     "anti-fascist",
     "anti-general_assembly",
     "anti-security_council",
@@ -92,17 +92,17 @@
     "steampunk",
     "surreal",
     "theocratic",
     "totalitarian",
     "trading_cards",
     "video_game",
     "world_assembly",
-]
+}
 
-nation_shards: list[str] = [
+NATION_SHARDS: set[str] = {
     "admirable",
     "admirables",
     "animal",
     "animaltrait",
     "answered",
     "banner",
     "banners",
@@ -163,30 +163,30 @@
     "tgcanrecruit",
     "tgcancampaign",
     "type",
     "wa",
     "wabadges",
     "wcensus",
     "zombie",
-]
+}
 
-private_nation_shards: list[str] = [
+PRIVATE_NATION_SHARDS: set[str] = {
     "dossier",
     "issues",
     "issuesummary",
     "nextissue",
     "nextissuetime",
     "notices",
     "packs",
     "ping",
     "rdossier",
     "unread",
-]
+}
 
-region_shards: list[str] = [
+REGION_SHARDS: set[str] = {
     "banlist",
     "banner",
     "bannerby",
     "bannerurl",
     "census",
     "censusranks",
     "dbid",
@@ -217,17 +217,17 @@
     "officers",
     "poll",
     "power",
     "scvote",
     "tags",
     "wabadges",
     "zombie",
-]
+}
 
-world_shards: list[str] = [
+WORLD_SHARDS: set[str] = {
     "banner",
     "census",
     "censusid",
     "censusdesc",
     "censusname",
     "censusranks",
     "censusscale",
@@ -243,23 +243,29 @@
     "newnations",
     "numnations",
     "numregions",
     "poll",
     "regions",
     "regionsbytag",
     "tgqueue",
-]
+}
 
-wa_shards: list[str] = [
+WA_SHARDS: set[str] = {
     "numnations",
     "numdelegates",
     "delegates",
     "members",
     "happenings",
     "proposals",
     "resolution",
     "voters",
     "votetrack",
     "dellog",
     "delvotes",
     "lastresolution",
-]
+}
+
+PRIVATE_COMMANDS: set[str] = {
+    "issue",
+    "giftcard",
+    "dispatch",
+}
```

### Comparing `nsdotpy-1.3.4/pyproject.toml` & `nsdotpy-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.3.4"
+version = "2.0.0"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 httpx = { extras = ["http2"], version = "^0.24.0" }
 beautifulsoup4 = "^4.12.2"
 keyboard = "^0.13.5"
 tendo = "^0.3.0"
 lxml = "^4.9.2"
+python-benedict = {extras = ["parse", "xml"], version = "^0.31.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pdoc = "^13.1.1"
 pyinstaller = "^5.10.1"
 
 [build-system]
```

### Comparing `nsdotpy-1.3.4/PKG-INFO` & `nsdotpy-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.3.4
+Version: 2.0.0
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: keyboard (>=0.13.5,<0.14.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: python-benedict[parse,xml] (>=0.31.0,<0.32.0)
 Requires-Dist: tendo (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/sw33ze/NSDotPy
 Description-Content-Type: text/markdown
 
 # NSDotPy
 
 A Python wrapper around httpx for legally interacting with the HTML NationStates site, as well as a barebones API client. Built for legality first and foremost, as well as ease of use.
@@ -32,14 +33,22 @@
 ```python
 
 from nsdotpy.session import NSSession
 session = NSSession("NSDotPy Example", "1.0.0", "Script Author's nation", "Script User's nation")
 
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
+
+# an API client is also available, here's a simple example
+data = session.api_request("world", shard="nations")
+# it returns a benedict object (https://github.com/fabiocaccamo/python-benedict), which is a dict with some extra features
+# you can access the data like a normal dict
+nations = data["nations"].split(",")
+# or you can use a keyattribute (my personal favorite)
+nations = data.nations.split(",")
 ```
 
 ## TODO:
 
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
```

