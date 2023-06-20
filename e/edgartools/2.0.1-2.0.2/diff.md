# Comparing `tmp/edgartools-2.0.1.tar.gz` & `tmp/edgartools-2.0.2.tar.gz`

## Comparing `edgartools-2.0.1.tar` & `edgartools-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/__about__.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/__init__.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_codes.py
--rw-r--r--   0        0        0    29821 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_companies.py
--rw-r--r--   0        0        0    61226 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_filings.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_gaap.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_markdown.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_party.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_rich.py
--rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_xbrl.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/_xml.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/core.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/effect.py
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/financials.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/form144.py
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/forms.py
--rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/fundreports.py
--rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/muniadvisors.py
--rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/offerings.py
--rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/ownership.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/search.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/shelfofferings.py
--rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.1/edgar/data/GAAP_Taxonomy_2022.csv
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0    19354 2020-02-02 00:00:00.000000 edgartools-2.0.1/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    20144 2020-02-02 00:00:00.000000 edgartools-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/__about__.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_codes.py
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_companies.py
+-rw-r--r--   0        0        0    69101 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_filings.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_gaap.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_markdown.py
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_party.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_rich.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_xbrl.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/_xml.py
+-rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/core.py
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/effect.py
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/financials.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/form144.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/forms.py
+-rw-r--r--   0        0        0    35794 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/fundreports.py
+-rw-r--r--   0        0        0    41031 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/muniadvisors.py
+-rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/offerings.py
+-rw-r--r--   0        0        0    27294 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/ownership.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/search.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/shelfofferings.py
+-rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-2.0.2/edgar/data/GAAP_Taxonomy_2022.csv
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 edgartools-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 edgartools-2.0.2/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edgartools-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    25209 2020-02-02 00:00:00.000000 edgartools-2.0.2/PKG-INFO
```

### Comparing `edgartools-2.0.1/edgar/__init__.py` & `edgartools-2.0.2/edgar/__init__.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_codes.py` & `edgartools-2.0.2/edgar/_codes.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_companies.py` & `edgartools-2.0.2/edgar/_companies.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,7 +823,8 @@
     def __init__(self,
                  data: pd.DataFrame):
         data = (data.drop_duplicates(subset='cik')
                 .set_index('cik')
                 .assign(company_idx=lambda df: np.vectorize(preprocess_company)(df.company))
                 )
         super().__init__(data, 'company_idx')
+
```

### Comparing `edgartools-2.0.1/edgar/_filings.py` & `edgartools-2.0.2/edgar/_filings.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 from edgar._markdown import MarkdownContent
 from edgar._markdown import html_to_markdown
 from edgar._rich import df_to_rich_table, repr_rich
 from edgar._xbrl import FilingXbrl
 from edgar._party import Address
 from edgar.core import (http_client, download_text, download_file, log, display_size, sec_edgar, get_text_between_tags,
-                        filter_by_date, sec_dot_gov, InvalidDateException, IntString, DataPager, text_extensions)
+                        filter_by_date, sec_dot_gov, InvalidDateException, IntString, DataPager, text_extensions,
+                        datefmt)
 from edgar.fundreports import FUND_FORMS
 from edgar.search import BM25Search, RegexSearch
 
 """ Contain functionality for working with SEC filing indexes and filings
 
 The module contains the following functions
 
@@ -329,14 +330,27 @@
     def filter(self,
                form: Union[str, List[IntString]] = None,
                amendments: bool = None,
                filing_date: str = None,
                date: str = None):
         """
         Filter the filings
+
+        On a date
+        >>> filings.filter(date="2020-01-01")
+
+        Up to a date
+        >>> filings.filter(date=":2020-03-01")
+
+        From a date
+        >>> filings.filter(date="2020-01-01:")
+
+        # Between dates
+        >>> filings.filter(date="2020-01-01:2020-03-01")
+
         :param form: The form or list of forms to filter by
         :param amendments: Whether to include amendments to the forms e.g include "10-K/A" if filtering for "10-K"
         :param filing_date: The filing date
         :param date: An alias for the filing date
         :return: The filtered filings
         """
         filing_index = self.data
@@ -594,23 +608,26 @@
 
 # Restricted stock sales
 get_restricted_stock_filings = partial(get_filings, form=[144])
 
 # Insider transaction filings
 get_insider_transaction_filings = partial(get_filings, form=[3, 4, 5])
 
+
 @lru_cache(maxsize=8)
 def _get_cached_filings(year: Years = None,
                         quarter: Quarters = None,
                         form: Union[str, List[IntString]] = None,
                         amendments: bool = True,
                         filing_date: str = None,
                         index="form") -> Filings:
     # Get the filings but cache the result
-    return get_filings(year=year,quarter=quarter,form=form,amendments=amendments,filing_date=filing_date,index=index)
+    return get_filings(year=year, quarter=quarter, form=form, amendments=amendments, filing_date=filing_date,
+                       index=index)
+
 
 def parse_filing_header(content):
     data = {}
     current_key = None
 
     lines = content.split('\n')
     for line in lines:
@@ -652,14 +669,44 @@
 class Filer:
     company_information: CompanyInformation
     filing_information: FilingInformation
     business_address: Address
     mailing_address: Address
     former_company_names: Optional[List[FormerCompany]] = None
 
+    def __rich__(self):
+        filer_table = Table("Company", "CIK", "SIC", "Incorp.", "Fiscal Year End",
+                            title=company_title,
+                            box=box.SIMPLE)
+        filer_table.add_row(self.company_information.name,
+                            self.company_information.cik,
+                            self.company_information.sic,
+                            self.company_information.state_of_incorporation,
+                            self.company_information.fiscal_year_end)
+
+        filer_renderables = [filer_table]
+        # Addresses
+        if self.business_address or self.mailing_address:
+            filer_renderables.append(_create_address_table(self.business_address, self.mailing_address))
+
+        # Former Company Names
+        if self.former_company_names:
+            former_company_table = Table("Former Company Name", "Date of Change", box=box.SIMPLE)
+            for company in self.former_company_names:
+                former_company_table.add_row(company.name, company.date_of_change)
+            filer_renderables.append(former_company_table)
+
+        return Panel(
+            Group(*filer_renderables),
+            title="FILER"
+        )
+
+    def __repr__(self):
+        return repr_rich(self.__rich__())
+
 
 @dataclass(frozen=True)
 class Owner:
     name: str
     cik: str
 
 
@@ -667,49 +714,155 @@
 class ReportingOwner:
     owner: Owner
     company_information: CompanyInformation
     filing_information: FilingInformation
     business_address: Address
     mailing_address: Address
 
+    def __rich__(self):
+        reporting_owner_renderables = []
+
+        # Owner Table
+        if self.owner:
+            reporting_owner_table = Table("Owner", "CIK", box=box.SIMPLE)
+            reporting_owner_table.add_row(self.owner.name, self.owner.cik)
+
+            reporting_owner_renderables = [reporting_owner_table]
+        # Reporting Owner Filing Values
+        if self.filing_information:
+            filing_values_table = Table("File Number", "SEC Act", "Film Number", box=box.SIMPLE)
+            filing_values_table.add_row(self.filing_information.file_number,
+                                        self.filing_information.sec_act,
+                                        self.filing_information.film_number)
+            reporting_owner_renderables.append(filing_values_table)
+
+        # Addresses
+        if self.business_address or self.mailing_address:
+            reporting_owner_renderables.append(_create_address_table(self.business_address, self.mailing_address))
+
+        return Panel(
+            Group(
+                *reporting_owner_renderables
+            ),
+            title=reporting_owner_title
+        )
+
+    def __repr__(self):
+        return repr_rich(self.__rich__())
+
+
 @dataclass(frozen=True)
 class SubjectCompany:
     company_information: CompanyInformation
     filing_information: FilingInformation
     business_address: Address
     mailing_address: Address
     former_company_names: Optional[List[FormerCompany]] = None
 
+    def __rich__(self):
+        company_information_table = Table("Company", "CIK", "SIC", "Fiscal Year End",
+                                          box=box.SIMPLE)
+        company_information_table.add_row(self.company_information.name,
+                                          self.company_information.cik,
+                                          self.company_information.sic,
+                                          self.company_information.fiscal_year_end)
+
+        subject_company_renderables = [company_information_table]
+
+        # Fiing Information
+        if self.filing_information:
+            filing_values_table = Table("File Number", "SEC Act", "Film Number", box=box.SIMPLE)
+            filing_values_table.add_row(self.filing_information.file_number,
+                                        self.filing_information.sec_act,
+                                        self.filing_information.film_number)
+            subject_company_renderables.append(filing_values_table)
+
+        # Addresses
+        if self.business_address or self.mailing_address:
+            subject_company_renderables.append(_create_address_table(self.business_address, self.mailing_address))
+
+        # Former Company Names
+        if self.former_company_names:
+            former_company_table = Table("Former Company Name", "Date of Change", box=box.SIMPLE)
+            for company in self.former_company_names:
+                former_company_table.add_row(company.name, company.date_of_change)
+            subject_company_renderables.append(former_company_table)
+
+        return Panel(
+            Group(
+                *subject_company_renderables
+            ),
+            title="SUBJECT COMPANY"
+        )
+
+    def __repr__(self):
+        return repr_rich(self.__rich__())
 
 @dataclass(frozen=True)
 class Issuer:
     company_information: CompanyInformation
     business_address: Address
     mailing_address: Address
 
+    def __rich__(self):
+        issuer_table = Table("Company", "CIK", "SIC", "Fiscal Year End",
+                             box=box.SIMPLE)
+        issuer_table.add_row(self.company_information.name,
+                             self.company_information.cik,
+                             self.company_information.sic,
+                             self.company_information.fiscal_year_end)
+
+        # The list of renderables for the issuer panel
+        issuer_renderables = [issuer_table]
+
+        # Addresses
+        if self.business_address or self.mailing_address:
+            issuer_renderables.append(_create_address_table(self.business_address, self.mailing_address))
+
+        return Panel(
+            Group(
+                *issuer_renderables
+            ),
+            title=issuer_title
+        )
+
+    def __repr__(self):
+        return repr_rich(self.__rich__())
+
 
 # Title text
 mailing_address_title = "\U0001F4EC Mailing Address"
 business_address_title = "\U0001F4EC Business Address"
-company_title = "\U0001F3E2 Company"
+company_title = "\U0001F3E2 Company Information"
 reporting_owner_title = "\U0001F468 REPORTING OWNER"
 issuer_title = "\U0001F4B5 ISSUER"
 filing_title = "\U0001F4D1 FILING"
 
 
-def _create_address_table(address: Address, title: str):
-    address_table = Table("Street1", "Street2", "City", "State", "Zipcode",
-                          title=title, box=box.SIMPLE)
-    address_table.add_row(address.street1,
-                          address.street2,
-                          address.city,
-                          address.state_or_country,
-                          address.zipcode)
+def _create_address_table(business_address: Address, mailing_address: Address):
+    address_table = Table("Type", "Street1", "Street2", "City", "State", "Zipcode",
+                          title="\U0001F4EC Addresses", box=box.SIMPLE)
+    if business_address:
+        address_table.add_row("\U0001F3E2 Business Address",
+                              business_address.street1,
+                              business_address.street2,
+                              business_address.city,
+                              business_address.state_or_country,
+                              business_address.zipcode)
+
+    if mailing_address:
+        address_table.add_row("\U0001F4ED Mailing Address",
+                              mailing_address.street1,
+                              mailing_address.street2,
+                              mailing_address.city,
+                              mailing_address.state_or_country,
+                              mailing_address.zipcode)
     return address_table
 
+
 class SECHeader:
     """
     Contains the parsed representation of the SEC-HEADER text at the top of the full submission text
     <SEC-HEADER>
 
     </SEC-HEADER>
     """
@@ -717,15 +870,15 @@
     def __init__(self,
                  header_text: str,
                  filing_metadata: Dict[str, str],
                  filers: List[Filer] = None,
                  reporting_owners: List[ReportingOwner] = None,
                  issuers: List[Issuer] = None,
                  subject_companies: List[SubjectCompany] = None):
-        self.header_text:str = header_text
+        self.header_text: str = header_text
         self.filing_metadata: Dict[str, str] = filing_metadata
         self.filers: List[Filer] = filers
         self.reporting_owners: List[ReportingOwner] = reporting_owners
         self.issuers: List[Issuer] = issuers
         self.subject_companies = subject_companies
 
     @property
@@ -751,15 +904,15 @@
     @property
     def acceptance_datetime(self):
         acceptance = self.filing_metadata.get("ACCEPTANCE-DATETIME")
         if acceptance:
             return datetime.strptime(acceptance, "%Y%m%d%H%M%S")
 
     @classmethod
-    def parse(cls, header_text:str):
+    def parse(cls, header_text: str):
         data = {}
         current_header = None
         current_subheader = None
 
         # Read the lines in the content. This starts with <ACCEPTANCE-DATETIME>20230606213204
         for line in header_text.split('\n'):
             if not line:
@@ -801,61 +954,61 @@
                         if current_subheader == "FORMER COMPANY":
                             data[current_header][-1][current_subheader][-1][key.strip()] = value
                         else:
                             data[current_header][-1][current_subheader][key.strip()] = value
 
         # The filer
         filers = []
-        for filer_values in data.get('FILER', []):
+        for filer_values in data.get('FILER', data.get('FILED BY', [])):
             filer_company_values = filer_values.get('COMPANY DATA')
             company_obj = None
             if filer_company_values:
-                    company_obj = CompanyInformation(
-                        name=filer_company_values.get('COMPANY CONFORMED NAME'),
-                        cik=filer_company_values.get('CENTRAL INDEX KEY'),
-                        sic=filer_company_values.get('STANDARD INDUSTRIAL CLASSIFICATION'),
-                        irs_number=filer_company_values.get('IRS NUMBER'),
-                        state_of_incorporation=filer_company_values.get('STATE OF INCORPORATION'),
-                        fiscal_year_end=filer_company_values.get('FISCAL YEAR END')
+                company_obj = CompanyInformation(
+                    name=filer_company_values.get('COMPANY CONFORMED NAME'),
+                    cik=filer_company_values.get('CENTRAL INDEX KEY'),
+                    sic=filer_company_values.get('STANDARD INDUSTRIAL CLASSIFICATION'),
+                    irs_number=filer_company_values.get('IRS NUMBER'),
+                    state_of_incorporation=filer_company_values.get('STATE OF INCORPORATION'),
+                    fiscal_year_end=filer_company_values.get('FISCAL YEAR END')
                 )
             # Filing Values
             filing_values_text_section = filer_values.get('FILING VALUES')
             filing_values_obj = None
             if filing_values_text_section:
-                    filing_values_obj = FilingInformation(
-                        form=filing_values_text_section.get('FORM TYPE'),
-                        sec_act=filing_values_text_section.get('SEC ACT'),
-                        file_number=filing_values_text_section.get('SEC FILE NUMBER'),
-                        film_number=filing_values_text_section.get('FILM NUMBER')
-                    )
-             # Now create the filer
+                filing_values_obj = FilingInformation(
+                    form=filing_values_text_section.get('FORM TYPE'),
+                    sec_act=filing_values_text_section.get('SEC ACT'),
+                    file_number=filing_values_text_section.get('SEC FILE NUMBER'),
+                    film_number=filing_values_text_section.get('FILM NUMBER')
+                )
+            # Now create the filer
             filer = Filer(
-                    company_information=company_obj,
-                    filing_information=filing_values_obj,
-                    business_address=Address(
-                        street1=filer_values['BUSINESS ADDRESS'].get('STREET 1'),
-                        street2=filer_values['BUSINESS ADDRESS'].get('STREET 2'),
-                        city=filer_values['BUSINESS ADDRESS'].get('CITY'),
-                        state_or_country=filer_values['BUSINESS ADDRESS'].get('STATE'),
-                        zipcode=filer_values['BUSINESS ADDRESS'].get('ZIP'),
+                company_information=company_obj,
+                filing_information=filing_values_obj,
+                business_address=Address(
+                    street1=filer_values['BUSINESS ADDRESS'].get('STREET 1'),
+                    street2=filer_values['BUSINESS ADDRESS'].get('STREET 2'),
+                    city=filer_values['BUSINESS ADDRESS'].get('CITY'),
+                    state_or_country=filer_values['BUSINESS ADDRESS'].get('STATE'),
+                    zipcode=filer_values['BUSINESS ADDRESS'].get('ZIP'),
 
-                    ) if 'BUSINESS ADDRESS' in filer_values else None,
-                    mailing_address=Address(
-                        street1=filer_values['MAIL ADDRESS'].get('STREET 1'),
-                        street2=filer_values['MAIL ADDRESS'].get('STREET 2'),
-                        city=filer_values['MAIL ADDRESS'].get('CITY'),
-                        state_or_country=filer_values['MAIL ADDRESS'].get('STATE'),
-                        zipcode=filer_values['MAIL ADDRESS'].get('ZIP'),
-
-                    ) if 'MAIL ADDRESS' in filer_values else None,
-                    former_company_names=[FormerCompany(date_of_change=record.get('DATE OF NAME CHANGE'),
-                                                        name=record.get('FORMER CONFORMED NAME'))
-                                          for record in filer_values['FORMER COMPANY']
-                                          ]
-                    if 'FORMER COMPANY' in filer_values else None
+                ) if 'BUSINESS ADDRESS' in filer_values else None,
+                mailing_address=Address(
+                    street1=filer_values['MAIL ADDRESS'].get('STREET 1'),
+                    street2=filer_values['MAIL ADDRESS'].get('STREET 2'),
+                    city=filer_values['MAIL ADDRESS'].get('CITY'),
+                    state_or_country=filer_values['MAIL ADDRESS'].get('STATE'),
+                    zipcode=filer_values['MAIL ADDRESS'].get('ZIP'),
+
+                ) if 'MAIL ADDRESS' in filer_values else None,
+                former_company_names=[FormerCompany(date_of_change=record.get('DATE OF NAME CHANGE'),
+                                                    name=record.get('FORMER CONFORMED NAME'))
+                                      for record in filer_values['FORMER COMPANY']
+                                      ]
+                if 'FORMER COMPANY' in filer_values else None
             )
             filers.append(filer)
 
         # Reporting Owner
 
         reporting_owners = []
 
@@ -898,37 +1051,37 @@
                 )
             reporting_owners.append(reporting_owner)
 
         # Issuer
         issuers = []
         for issuer_values in data.get('ISSUER', []):
             issuer = Issuer(
-                    company_information=CompanyInformation(
-                        name=issuer_values.get('COMPANY DATA').get('COMPANY CONFORMED NAME'),
-                        cik=issuer_values.get('COMPANY DATA').get('CENTRAL INDEX KEY'),
-                        sic=issuer_values.get('COMPANY DATA').get('STANDARD INDUSTRIAL CLASSIFICATION'),
-                        irs_number=issuer_values.get('COMPANY DATA').get('IRS NUMBER'),
-                        state_of_incorporation=issuer_values.get('COMPANY DATA').get('STATE OF INCORPORATION'),
-                        fiscal_year_end=issuer_values.get('COMPANY DATA').get('FISCAL YEAR END')
-                    ) if 'COMPANY DATA' in issuer_values else None,
-                    business_address=Address(
-                        street1=issuer_values.get('BUSINESS ADDRESS').get('STREET 1'),
-                        street2=issuer_values.get('BUSINESS ADDRESS').get('STREET 2'),
-                        city=issuer_values.get('BUSINESS ADDRESS').get('CITY'),
-                        state_or_country=issuer_values.get('BUSINESS ADDRESS').get('STATE'),
-                        zipcode=issuer_values.get('BUSINESS ADDRESS').get('ZIP'),
-                    ) if 'BUSINESS ADDRESS' in issuer_values else None,
-                    mailing_address=Address(
-                        street1=issuer_values.get('MAIL ADDRESS').get('STREET 1'),
-                        street2=issuer_values.get('MAIL ADDRESS').get('STREET 2'),
-                        city=issuer_values.get('MAIL ADDRESS').get('CITY'),
-                        state_or_country=issuer_values.get('MAIL ADDRESS').get('STATE'),
-                        zipcode=issuer_values.get('MAIL ADDRESS').get('ZIP'),
-                    ) if 'MAIL ADDRESS' in issuer_values else None
-                )
+                company_information=CompanyInformation(
+                    name=issuer_values.get('COMPANY DATA').get('COMPANY CONFORMED NAME'),
+                    cik=issuer_values.get('COMPANY DATA').get('CENTRAL INDEX KEY'),
+                    sic=issuer_values.get('COMPANY DATA').get('STANDARD INDUSTRIAL CLASSIFICATION'),
+                    irs_number=issuer_values.get('COMPANY DATA').get('IRS NUMBER'),
+                    state_of_incorporation=issuer_values.get('COMPANY DATA').get('STATE OF INCORPORATION'),
+                    fiscal_year_end=issuer_values.get('COMPANY DATA').get('FISCAL YEAR END')
+                ) if 'COMPANY DATA' in issuer_values else None,
+                business_address=Address(
+                    street1=issuer_values.get('BUSINESS ADDRESS').get('STREET 1'),
+                    street2=issuer_values.get('BUSINESS ADDRESS').get('STREET 2'),
+                    city=issuer_values.get('BUSINESS ADDRESS').get('CITY'),
+                    state_or_country=issuer_values.get('BUSINESS ADDRESS').get('STATE'),
+                    zipcode=issuer_values.get('BUSINESS ADDRESS').get('ZIP'),
+                ) if 'BUSINESS ADDRESS' in issuer_values else None,
+                mailing_address=Address(
+                    street1=issuer_values.get('MAIL ADDRESS').get('STREET 1'),
+                    street2=issuer_values.get('MAIL ADDRESS').get('STREET 2'),
+                    city=issuer_values.get('MAIL ADDRESS').get('CITY'),
+                    state_or_country=issuer_values.get('MAIL ADDRESS').get('STATE'),
+                    zipcode=issuer_values.get('MAIL ADDRESS').get('ZIP'),
+                ) if 'MAIL ADDRESS' in issuer_values else None
+            )
             issuers.append(issuer)
 
         subject_companies = []
         for subject_company_values in data.get('SUBJECT COMPANY', []):
             subject_company = SubjectCompany(
                 company_information=CompanyInformation(
                     name=subject_company_values.get('COMPANY DATA').get('COMPANY CONFORMED NAME'),
@@ -968,15 +1121,15 @@
             subject_companies.append(subject_company)
 
         # Create a dict of the values in data that are not nested dicts
         filing_metadata = {key: value for key, value in data.items() if isinstance(value, str)}
 
         # The header text contains <ACCEPTANCE-DATETIME>20230612172243. Replace with the formatted date
         header_text = re.sub(r'<ACCEPTANCE-DATETIME>(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})(\d{2})',
-               r'ACCEPTANCE-DATETIME:            \1-\2-\3 \4:\5:\6', header_text)
+                             r'ACCEPTANCE-DATETIME:            \1-\2-\3 \4:\5:\6', header_text)
 
         # Remove empty lines from header_text
         header_text = '\n'.join([line for line in header_text.split('\n') if line.strip()])
 
         # Create the Filing object
         return cls(
             header_text=header_text,
@@ -984,15 +1137,55 @@
             filers=filers,
             reporting_owners=reporting_owners,
             issuers=issuers,
             subject_companies=subject_companies
         )
 
     def __rich__(self):
-        return Panel(Text(self.header_text))
+
+        # Filing Metadata
+        metadata_table = Table(row_styles=["bold", ""], box=box.ROUNDED)
+        metadata_table.add_column("")
+        metadata_table.add_column("Value", style="bold")
+        for key, value in self.filing_metadata.items():
+            # Format as dates
+            if re.match(r"^(20|19)\d{12}$", value):
+                value = datefmt(value, "%Y-%m-%d %H:%M:%S")
+            elif re.match(r"^(20|19)\d{6}$", value):
+                value = datefmt(value, "%Y-%m-%d")
+
+            metadata_table.add_row(f"{key}:", value)
+
+        metadata_panel = Panel(
+            metadata_table, title=f"Form {self.form} {unicode_for_form(self.form)} FILING"
+        )
+
+        # Keep a list of renderables for rich
+        renderables = [metadata_panel]
+
+        # SUBJECT COMPANY
+        for subject_company in self.subject_companies:
+            renderables.append(subject_company.__rich__())
+
+        # FILER
+        for filer in self.filers:
+            renderables.append(filer.__rich__())
+
+        # REPORTING OWNER
+        for reporting_owner in self.reporting_owners:
+            renderables.append(reporting_owner.__rich__())
+
+        # ISSUER
+        for issuer in self.issuers:
+            renderables.append(issuer.__rich__())
+        return Panel(
+            Group(
+                *renderables
+            )
+        )
 
     def __repr__(self):
         return repr_rich(self.__rich__())
 
 
 class Filing:
     """
@@ -1168,18 +1361,18 @@
         return isinstance(other, Filing) and self.accession_no == other.accession_no
 
     def __ne__(self, other):
         return not self == other
 
     def summary(self) -> pd.DataFrame:
         """Return a summary of this filing as a dataframe"""
-        return pd.DataFrame([{"accession_no": self.accession_no,
-                              "Filed on": self.filing_date,
+        return pd.DataFrame([{"Accession Number": self.accession_no,
+                              "Filing Date": self.filing_date,
                               "Company": self.company,
-                              "CIK": self.cik}]).set_index("accession_no")
+                              "CIK": self.cik}]).set_index("Accession Number")
 
     def __str__(self):
         """
         Return a string version of this filing e.g.
 
         Filing(form='10-K', filing_date='2018-03-08', company='CARBO CERAMICS INC',
               cik=1009672, accession_no='0001564590-18-004771')
@@ -1449,14 +1642,15 @@
 
         # It is html so use "html.parser" (instead of "xml", or "lxml")
         soup = BeautifulSoup(homepage_html, features="html.parser")
 
         # Keep track of the tables as dataframes so we can append later
         dfs = []
 
+        # The table containin the attachments
         tables = soup.find_all("table", class_="tableFile")
         for table in tables:
             summary = table.attrs.get("summary")
             rows = table.find_all("tr")
             column_names = [th.text for th in rows[0].find_all("th")] + ["Url"]
             records = []
 
@@ -1473,37 +1667,48 @@
                            .assign(table=summary)
                            )
             dfs.append(table_as_df)
 
         # Now concat into a single dataframe
         files = pd.concat(dfs, ignore_index=True)
 
+        # The table containing the contract series
+
+        """
+        table_series = soup.find("table", class_="tableSeries")
+        TODO: Implement Table Series
+        if table_series:
+            for row in table_series.find_all("tr"):
+                cells = row.find_all("td")
+                print(cells)
+         """
+
         return cls(files,
                    url=url,
                    filing=filing)
 
     def __str__(self):
         return f"Homepage for {self.description}"
 
     def __repr__(self):
         return repr_rich(self.__rich__())
 
     def __rich__(self):
-        return Group(
+        return Panel(Group(
             Text(f"{self.filing.form} filing", style="bold"),
-            df_to_rich_table(self.filing.summary(), index_name="accession_no"),
+            df_to_rich_table(self.filing.summary(), index_name="Accession Number"),
             Group(Text("Documents", style="bold"),
                   df_to_rich_table(summarize_files(self.documents), index_name="Seq")
                   ),
             Group(Text("Datafiles", style="bold"),
                   df_to_rich_table(
                       summarize_files(self.datafiles), index_name="Seq"),
                   ) if self.datafiles is not None else Text(""),
 
-        )
+        ), title=f"{self.filing.form} filing            Accession Number: {self.filing.accession_no}")
 
 
 def summarize_files(data: pd.DataFrame) -> pd.DataFrame:
     return (data
             .filter(["Seq", "Document", "Description", "Size"])
             .assign(Size=data.Size.apply(display_size))
             .set_index("Seq")
```

### Comparing `edgartools-2.0.1/edgar/_gaap.py` & `edgartools-2.0.2/edgar/_gaap.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_markdown.py` & `edgartools-2.0.2/edgar/_markdown.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_party.py` & `edgartools-2.0.2/edgar/_party.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_rich.py` & `edgartools-2.0.2/edgar/_rich.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_xbrl.py` & `edgartools-2.0.2/edgar/_xbrl.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/_xml.py` & `edgartools-2.0.2/edgar/_xml.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/core.py` & `edgartools-2.0.2/edgar/core.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/effect.py` & `edgartools-2.0.2/edgar/effect.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/financials.py` & `edgartools-2.0.2/edgar/financials.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/form144.py` & `edgartools-2.0.2/edgar/form144.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/forms.py` & `edgartools-2.0.2/edgar/forms.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/fundreports.py` & `edgartools-2.0.2/edgar/fundreports.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/muniadvisors.py` & `edgartools-2.0.2/edgar/muniadvisors.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/offerings.py` & `edgartools-2.0.2/edgar/offerings.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/ownership.py` & `edgartools-2.0.2/edgar/ownership.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/search.py` & `edgartools-2.0.2/edgar/search.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/edgar/data/GAAP_Taxonomy_2022.csv` & `edgartools-2.0.2/edgar/data/GAAP_Taxonomy_2022.csv`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/LICENSE.txt` & `edgartools-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgartools-2.0.1/README.md` & `edgartools-2.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,571 +1,657 @@
-
-
-![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/main/images/edgar-tools.png)
-
-[![PyPI - Version](https://img.shields.io/pypi/v/edgartools.svg)](https://pypi.org/project/edgartools)
-![GitHub last commit](https://img.shields.io/github/last-commit/dgunning/edgartools)
-![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dgunning/edgartools/python-hatch-workflow.yml)
-[![CodeFactor](https://www.codefactor.io/repository/github/dgunning/edgartools/badge)](https://www.codefactor.io/repository/github/dgunning/edgartools)
-[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
-![GitHub](https://img.shields.io/github/license/dgunning/edgartools)
------
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#demo">Demo</a></li>
-        <li><a href="#features">Features</a></li>
-      </ul>
-    </li>
-    <li>
-        <a href="#installation">Installation</a>
-    </li>
-    <li>
-        <a href="#usage">Usage</a>
-        <ul>
-            <li><a href="#set-your-edgar-user-identity">Set your Edgar user identity</a></li>
-            <li><a href="#getting-filings">Getting Filings</a></li>
-            <li><a href="#using-the-company-api">Using the Company API</a></li>
-      </ul>
-    </li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-  </ol>
-</details>
-
-# About the project
-
-**`edgartools`** is one of the nicest looking EDGAR libraries out there.
-You can query, filter and select any filing since 1994 and view the filing's html, text, xml or structured data.
-
-
-## Demo
-
-#### Show 20 10-K filings for the 2nd quarter of 2023 and open the first in the browser
-
-```python
-from edgar import *
-
-# Get 10-K filings for the second quarter of 2023 
-ten_k_filings = get_filings(2023, 2, form="10-K")
-
-# Get the latest 20 filings from the list 
-latest_ten_k_filings = filings.latest(20)
-
-# Open the 1st filing in the browser
-latest_ten_k_filings[0].open()
-```
-
-![10 K Filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_10K_filings.png)
-
-
-## Features
-
-### Start with filings, filter down to a filing
-
-- View filings since 1994 to today
-- Filter filings by **form e.g. 10K**, **filing date** etc.
-- Page through filings using **next()** and **prev()**
-- Select and view a filing in the terminal, or open in the browser
-- Download any file from any filing
-- Parse XML for **Offering, Ownership** and other filing types
-- Automatically parse a filing's XBRL into a pandas dataframe
-
-### Start with a Company, get their filings and Facts
-- Search for company by ticker or CIK
-- View a company's filings
-- Page through filings using **next()** and **prev()**
-- Get a company **facts** e.g. **CommonSharesOutstanding** as a dataframe
-
-# Installation
-
-```console
-pip install edgartools
-```
-
-# Usage
-
-
-## Set your Edgar user identity
-
-Before you can access the SEC Edgar API you need to set the identity that you will use to access Edgar.
-This is usually your name and email, or a company name and email.
-```bash
-Sample Company Name AdminContact@<sample company domain>.com
-```
-
-The user identity is sent in the User-Agent string and the Edgar API will refuse to respond to your request without it.
-
-EdgarTools will look for an environment variable called `EDGAR_IDENTITY` and use that in each request.
-So, you need to set this environment variable before using it.
-
-### Setting EDGAR_IDENTITY in Linux/Mac
-```bash
-export EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com"
-```
-
-### Setting EDGAR_IDENTITY in Windows Powershell
-```bash
- $Env:EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com"
-```
-Alternatively, you can call `set_identity` which does the same thing.
-
-```python
-from edgar import set_identity
-set_identity("Michael Mccallum mcalum@gmail.com")
-```
-For more detail see https://www.sec.gov/os/accessing-edgar-data
-
-## Usage
-
-### Importing edgar
-
-```python
-from edgar import *
-```
-
-### Getting filings
-```python
-
-# Get filings for the current year and quarter
-filings = get_filings() 
-
-# Get filings for 2022
-filings = get_filings(2022)                 # OR filings = get_filings(year=2022)
-
-# Get filings for 2022 quarter 4
-filings = get_filings(2022, 4)              # OR filings = get_filings(year=2022, quarter=4)
-
-# Get filings for 2020, 2021 and 2022
-filings = get_filings([2020, 2021, 2022])   # OR filings = get_filings(year=range(2020, 2023))
-
-# Get filings for 2020 quarters 1 and 2
-filings = get_filings(2020, quarter=[1,2])
-```
-![Get filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/get_filings.jpg)
-
-
-
-### Filtering filings
-
-```python
-# Filter for form D
-filings.filter(form="D")
-
-# Filter for form 10-K and 10-Q 
-filings.filter(form=["10-K", "10-Q"])
-
-# When you filter by form e.g. "D" it includes amendments e.g. "D\A". You can omit amendments
-filings.filter(form="D", amendments=False)
-
-# Filter by filing_date. date and filing_date mean the same thing
-# Get all filings on 2023-02-23
-filings.filter(date="2023-02-23")                      
-# OR
-filings.filter(filing_date="2023-02-23")
-
-# Filter to get all filings between 2023-01-23 and 2023-02-23     
-filings.filter(date="2023-01-23:2023-02-23")
-
-# Filter to get all filings since 2023-01-23   
-filings.filter(date="2023-01-23")
-
-# Filter to get all filings before 2023-02-23     
-filings.filter(date=":2023-02-23")
-```
-
-### Combining getting and filtering
-```python
-get_filings(2022, form="D")
-```
-
-### Convert the filings to a pandas dataframe
-
-The filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get the data as a pandas dataframe using
-`to_pandas`
-```python
-df = filings.to_pandas()
-```
-
-
-## Navigating filings
-
-The Filings object allows you to navigate through filings using `filings.next()` and `filings.prev()`. 
-This shows you pages of the data - the page size is about 50. 
-
-```python
-# To see the next page of data
-filings.next()
-
-# To see the previous page
-filings.prev()
-
-# To see the current page
-filings.current()
-```
-
-![Get next filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filings_next.jpg)
-
-## Getting the latest filings
-
-You can get the latest **n** filings by filing_date from a filings using `filings.latest()`.
-
-If you provide the parameter `n` it will return the latest `n` filings.
-
-```python
-filing = filings.latest(n=5)
-filing
-```
-![Latest filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filings.jpg)
-
-
-If you omit this parameter, or set `n=1` it will return a single `Filings object.
-
-```python
-filing = filings.latest()
-filing
-```
-![Latest filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filing.jpg)
-
-
-## Filtering filings
-
-You can filter the filings object using te `filter()` function. This allows you to filter
-by filing date, or by form.
-
-### Filtering filings by date
-
-To filter by filing date specify the filing date in **YYYY-MM-DD** format e.g. **2022-01-24**
-(Note the parameters `date` and `filing_date` are equivalent aliases for each other)
-```python
-filings.filter(date="2021-01-24") # or filings.filter(filing_date="2021-01-24")
-```
-You can specify a filing date range using the colon
-
-```python
-filings.filter(date="2021-01-12:2021-02-28") 
-```
-To filter by dates before a specified date use `:YYYY-MM-DD'
-
-```python
-filings.filter(date=":2021-02-28") 
-```
-
-To filter by dates after a specified date use `YYYY-MM-DD:'
-
-```python
-filings.filter(date="2021-02-28:") 
-```
-
-### Filtering filings by form
-
-You can filter filings by form using the `form` parameter. 
-
-```python
-filings.filter(form="10-K") 
-```
-
-To filter by form e.g. **10-K** and include form amendments use `amendments = True`. 
-
-```python
-filings.filter(form="10-K", amendments=True) 
-```
-![Filter with amendments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filter_amendments.jpg)
-
-## Getting a single filing
-
-You can get a single filing from the filings using the bracket operator `[]`, 
-specifying the index of the filing. The index is the value displayed in the leftmost
-position in the filings table. For example, to get the **10-Q** for **Costco** in the table above
-use `filings[3]`
-
-```python
-filing = filings[3]
-```
-
-![Costco 10Q filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/costco_10Q.jpg)
-
-### View the filing homepage
-You can view the filing homepage in the terminal using `filing.homepage`
-
-This gives you access to the `FilingHomepage` class that you can use to list all the documents
-and datafiles on the filing.
-
-```python
-filing.homepage
-```
-![Filing homepage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_homepage.jpg)
-
-### Open a filing
-
-You can open the filing in your browser using `filing.open()`. This will work on environments with access to the browser, 
-will probably not work on a remote server.
-```python
-filing.open()
-```
-
-### Open the Filing Homepage
-You can open the filing homepage in the browser using `filing.homepage.open()`.
-```python
-filing.homepage.open()
-```
-
-### View the filing as Markdown
-You can view the filing's HTML content as markdown in the console using `view()`. It works for all filing types
-but can be a little slow for filings with large HTML files
-```python
-filing.view()
-```
-
-### Get the filing's html
-You can get the html content of the filing using`.html()`
-```python
-filing.html()
-```
-
-### Get the filing's html as Markdown
-You can get the html content as markdown using`.markdown()`
-```python
-filing.markdown()
-```
-
-## Viewing and downloading attachments
-
-Every filing has a list of attachments. You can view the attachments using `filing.attachments`
-
-```python
-# View the attachments
-filing.attachments
-```
-![Filing attachments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_attachments.png)
-
-You can access each attachment using the bracket operator `[]` and the index of the attachment.
-    
-```python
-# Get the first attachment
-attachment = filing.attachments[0]
-```
-
-![Filing attachments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_attachment.png)
-
-You can download the attachment using `attachment.download()`. This will download the attachment to string or bytes in memory. 
-
-## Automatic parsing of filing data
-
-Now the reason you may want to download attachments is to get information contained in data files.
-For example, **13F-HR** filings have attached infotable.xml files containing data from the holding report for that filing.
-
-Fortunately, the library handles this for you. If you call `filing.obj()` it will automatically download and parse the data files
-into a data object, for several different form types. Currently, the following forms are supported:
-
-| Form                       | Data Object            | Description                           |
-|----------------------------|------------------------|---------------------------------------|
-| 10-K                       | `TenK`                 | Annual report                         |
-| 10-Q                       | `TenQ`                 | Quarterly report                      |
-| 8-K                        | `EightK`               | Current report                        |
-| MA-I                       | `MunicipalAdvisorForm` | Municipal advisor initial filing      |
-| Form 144                   | `Form144`              | Notice of proposed sale of securities |
-| D                          | `Offering`             | Offerings                             |
-| 3,4,5                      | `Ownership`            | Ownership reports                     |
-| 13F-HR                     | `ThirteenF`             | 13F Holdings Report                   |
-| NPORT-P                    | `FundReport`           | Fund Report                           |
-| EFFECT                     | `Effect`               | Notice of Effectiveness               |
-| And other filing with XBRL | `FilingXbrl`            ||
-
-For example, to get the data object for a **13F-HR** filing you can do the following:
-
-```python
-filings = get_filings(form="13F-HR")
-filing = filings[0]
-thirteenf = filing.obj()
-```
-
-![Filing attachments](images/thirteenF.png)
-
-If you call `obj()` on a filing that does not have a data file, then it will return `None`.
-
-
-## Working with XBRL filings
-
-Some filings are in **XBRL (eXtensible Business Markup Language)** format. 
-These are mainly the newer filings, as the SEC has started requiring this for newer filings.
-
-If a filing is in XBRL format then it opens up a lot more ways to get structured data about that specific filing and also 
-about the company referred to in that filing.
-
-The `Filing` class has an `xbrl` function that will download, parse and structure the filing's XBRL document if one exists.
-If it does not exist, then `filing.xbrl()` will return `None`.
-
-The function `filing.xbrl()` returns a `FilingXbrl` instance, which wraps the data, and provides convenient
-ways of working with the xbrl data.
-
-
-```python
-filing_xbrl = filing.xbrl()
-```
-
-![Filing homapage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/10Q_xbrl.jpg)
-
-
-## Using the Company API
-
-With the company API you find a company using the **cik** or **ticker**. 
-From the company you can access all their historical **filings**,
-and a dataset of the company **facts**.
-The SEC's company API also supplies a lot more details about a company including industry, the SEC filer type,
-the mailing and business address and much more.
-
-### Find a company using the cik
-The **cik** is the id that uniquely identifies a company at the SEC.
-It is a number, but is sometimes shown in SEC Edgar resources as a string padded with leading zero's.
-For the edgar client API, just use the numbers and omit the leading zeroes.
-
-```python
-company = Company(1324424)
-```
-![expe](https://raw.githubusercontent.com/dgunning/edgartools/main/images/expe.png)
-
-
-
-### Find a company using ticker
-
-You can get a company using a ticker e.g. **SNOW**. This will do a lookup for the company cik using the ticker, then load the company using the cik.
-This makes it two calls versus one for the cik company lookup, but is sometimes more convenient since tickers are easier to remember that ciks.
-
-Note that some companies have multiple tickers, so you technically cannot get SEC filings for a ticker.
-You instead get the SEC filings for the company to which the ticker belongs.
-
-The ticker is case-insensitive so you can use `Company("snow")`
-or `Company("SNOW")`
-```python
-snow = Company("snow")
-```
-
-![snow](https://raw.githubusercontent.com/dgunning/edgartools/main/images/snow.jpg)
-### 
-
-
-```python
-Company(1832950)
-```
-
-### Get filings for a company
-To get the company's filings use `get_filings()`. This gets all the company's filings that are available from the Edgar submissions endpoint.
-
-```python
-company.get_filings()
-```
-### Filtering filings
-You can filter the company filings using a number of different parameters.
-
-```python
-class CompanyFilings:
-    
-    ...
-    
-    def get_filings(self,
-                    *,
-                    form: str | List = None,
-                    accession_number: str | List = None,
-                    file_number: str | List = None,
-                    is_xbrl: bool = None,
-                    is_inline_xbrl: bool = None
-                    ):
-        """
-        Get the company's filings and optionally filter by multiple criteria
-        :param form: The form as a string e.g. '10-K' or List of strings ['10-Q', '10-K']
-        :param accession_number: The accession number that uniquely identifies an SEC filing e.g. 0001640147-22-000100
-        :param file_number: The file number e.g. 001-39504
-        :param is_xbrl: Whether the filing is xbrl
-        :param is_inline_xbrl: Whether the filing is inline_xbrl
-        :return: The CompanyFiling instance with the filings that match the filters
-        """
-```
-
-
-#### The CompanyFilings class
-The result of `get_filings()` is a `CompanyFilings` class. This class contains a pyarrow table with the filings
-and provides convenient functions for working with filings.
-You can access the underlying pyarrow `Table` using the `.data` property
-
-```python
-filings = company.get_filings()
-
-# Get the underlying Table
-data: pa.Table = filings.data
-```
-
-#### Get a filing by index
-To access a filing in the CompanyFilings use the bracket `[]` notation e.g. `filings[2]`
-```python
-filings[2]
-```
-
-#### Get the latest filing
-
-The `CompanyFilings` class has a `latest` function that will return the latest `Filing`. 
-So, to get the latest **10-Q** filing, you do the following
-```python
-# Latest filing makes sense if you filter by form  type e.g. 10-Q
-snow_10Qs = snow.get_filings(form='10-Q')
-latest_10Q = snow_10Qs.latest()
-
-# Or chain the function calls
-snow.get_filings(form='10-Q').latest()
-```
-
-
-### Get company facts
-
-Facts are an interesting and important dataset about a company accumlated from data the company provides to the SEC.
-Company facts are available for a company on the Company Facts`f"https://data.sec.gov/api/xbrl/companyfacts/CIK{cik:010}.json"`
-It is a JSON endpoint and `edgartools` parses the JSON into a structured dataset - a `pyarrow.Table`.
-
-#### Getting facts for a company
-To get company facts, first get the company, then call `company.get_facts()`
-```python
-company = Company("SNOW")
-company_facts = company.get_facts()
-```
-The result is a `CompanyFacts` object which wraps the underlying facts and provides convenient ways of working
-with the facts data. To get access to the underyling data use the `facts` property.
-
-You can get the facts as a pandas dataframe by calling `to_pandas`
-
-```python
-df = company_facts.to_pandas()
-```
-
-Facts differ among companies. To see what facts are available you can use the `facts_meta` property.
-
-
-# Contributing
-
-Contributions are welcome! We would love to hear your thoughts on how this library could be better at working with SEC Edgar.
-
-## Reporting Issues
-We use GitHub issues to track public bugs. 
-Report a bug by [opening a new issue](https://github.com/dgunning/edgartools/issues); it's that easy!
-
-## Making code changes
-- Fork the repo and create your branch from master.
-- If you've added code that should be tested, add tests.
-- If you've changed APIs, update the documentation.
-- Ensure the test suite passes.
-- Make sure your code lints.
-- Issue that pull request!
-
-
-
-# License
-
-`edgartools` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-## Contact
-
+Metadata-Version: 2.1
+Name: edgartools
+Version: 2.0.2
+Summary: One of the nicest looking EDGAR libraries out there
+Project-URL: Documentation, https://dgunning.github.io/edgartools/
+Project-URL: Issues, https://github.com/dgunning/edgartools/issues
+Project-URL: Source, https://github.com/dgunning/edgartools
+Author-email: Dwight Gunning <dgunning@gmail.com>
+License-File: LICENSE.txt
+Keywords: company,edgar,filings,finance,financial,python,reports,sec
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: beautifulsoup4>=4.10.0
+Requires-Dist: charset-normalizer>=2.1.1
+Requires-Dist: fastcore>=1.5.20
+Requires-Dist: httpx>=0.23.1
+Requires-Dist: humanize>=4.0.0
+Requires-Dist: lxml>=4.4
+Requires-Dist: markdownify>0.11.0
+Requires-Dist: pandas>=1.3.0
+Requires-Dist: pyarrow>=11.0.0
+Requires-Dist: rank-bm25==0.2.1
+Requires-Dist: retry>=0.9.2
+Requires-Dist: rich>=13.0.0
+Requires-Dist: textdistance>=4.5.0
+Description-Content-Type: text/markdown
+
+
+
+![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/main/images/edgar-tools.png)
+
+[![PyPI - Version](https://img.shields.io/pypi/v/edgartools.svg)](https://pypi.org/project/edgartools)
+![GitHub last commit](https://img.shields.io/github/last-commit/dgunning/edgartools)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dgunning/edgartools/python-hatch-workflow.yml)
+[![CodeFactor](https://www.codefactor.io/repository/github/dgunning/edgartools/badge)](https://www.codefactor.io/repository/github/dgunning/edgartools)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+![GitHub](https://img.shields.io/github/license/dgunning/edgartools)
+-----
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#demo">Demo</a></li>
+        <li><a href="#features">Features</a></li>
+      </ul>
+    </li>
+    <li>
+        <a href="#installation">Installation</a>
+    </li>
+    <li>
+        <a href="#usage">Usage</a>
+        <ul>
+            <li><a href="#set-your-edgar-user-identity">Set your Edgar user identity</a></li>
+            <li><a href="#getting-filings">Getting Filings</a></li>
+            <li><a href="#using-the-company-api">Using the Company API</a></li>
+      </ul>
+    </li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+  </ol>
+</details>
+
+# About the project
+
+**`edgartools`** is one of the nicest looking EDGAR libraries out there. It is also powerful and easy to use.
+You can query, filter and select any filing since 1994 and view the filing's html, text, xml or structured data.
+
+
+## Demo
+
+#### Show 20 10-K filings for the 2nd quarter of 2023 and open the first in the browser
+
+```python
+from edgar import *
+
+# Get 10-K filings for the second quarter of 2023 
+ten_k_filings = get_filings(2023, 2, form="10-K")
+
+# Get the latest 20 filings by date 
+latest_ten_k_filings = filings.latest(20)
+
+# Show the first filing 
+latest_ten_k_filings[0]
+```
+![10 K Filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_10K_filing.png)
+
+
+## Features
+
+### Getting started
+
+| Task                                 | Code                                                  |
+|--------------------------------------|-------------------------------------------------------|
+| Set your EDGAR identity in Linux/Mac | `export EDGAR_IDENTITY="First Last email@domain.com"` |
+| Set your EDGAR identity in Windows   | `set EDGAR_IDENTITY="First Last email@domain.com"`    |
+| Set identity in Windows Powershell   | `$env:EDGAR_IDENTITY="First Last email@domain.com"`   |
+| Set identity in Python               | `set_identity("First Last email@domain.com")`         |
+| Importing the library                | `from edgar import *`                                 |
+
+### Working with filings
+
+| Task                               | Code                                          |
+|------------------------------------|-----------------------------------------------|
+| Get filings for the year to date   | `filings = get_filings()`                     |
+| Get only xbrl filings              | `filings = get_filings(index="xbrl")`         |
+| Get filings for a specific year    | `filings = get_filings(2020)`                 |
+| Get filings for a specific quarter | `filings = get_filings(2020, 1)`              |
+| Get filings for multiple years     | `filings = get_filings([2020, 2021])`         |
+| Get filigs for a range of years    | `filings = get_filings(year=range(2010, 2020)` |
+| Get filings for a specific form    | `filings = get_filings(form="10-K")`          |
+| Get filings for a list of forms    | `filings = get_filings(form=["10-K", "10-Q"])` |
+| Show the next page of filings      | `filings.next()`                              |
+| Show the previous page of filings  | `filings.prev()`                              |
+| Get the first n filings            | `filings.head(20)`                            |
+| Get the last n filings             | `filings.tail(20)`                            |
+| Get the latest n filings by date   | `filings.latest(20)`                          |
+| Get a random sample of the filings | `filings.sample(20)`                          |
+| Filter filings on a date           | `filings = filings.filter(date="2020-01-01")` |
+| Filter filings between dates       | `filings.filter(date="2020-01-01:2020-03-01")` |
+| Filter filings before a date       | `filings.filter(date=":2020-03-01")`          |  
+| Filter filings after a date        | `filings.filter(date="2020-03-01:")`          |
+| Get filings as a pandas dataframe  | `filings.to_pandas()`                         |
+
+### Working with a filing
+
+| Task                                      | Code                                                      |
+|-------------------------------------------|-----------------------------------------------------------|
+| Get a single filing                       | `filing = filings[3]`                                     |
+| Get a filing by accession number          | `filing = get_by_accession_number("0000320193-20-34576")` |
+| Get the filing homepage                   | `filing.homepage`                                         |
+| Open a filing in the browser              | `filing.open()`                                           |
+| Open the filing homepage in the browser   | `filing.homepage.open()`                                  |
+| View the filing in the terminal           | `filing.view()`                                           |
+| Get the html of the filing document       | `filing.html()`                                           |
+| Get the XBRL of the filing document       | `filing.xbrl()`                                           |
+| Get the filing document as markdown       | `filing.markdown()`                                       |
+| Get the full submission text of a filing  | `filing.text()`                                           |
+| Get and parse the data object of a filing | `filing.obj()`                                            |
+| Get the filing attachments                | `filing.attachments`                                      |
+| Get a single attachment                   | `attachment = filing.attachments[0]`                      |
+| Open an attachment in the browser         | `attachment.open()`                                       |
+| Download an attachment                    | `content = attachment.download()`                         |
+
+### Working with a company
+
+| Task                                     | Code                                                          |
+|------------------------------------------|---------------------------------------------------------------|
+| Get a company by ticker                  | `company = Company("AAPL")`                                   |
+| Get a company by CIK                     | `company = Company("0000320193")`                             |
+| Get company facts                        | `company.get_facts()`                                         |
+| Get company facts as a pandas dataframe  | `company.get_facts().to_pandas()`                             |
+| Get company filings                      | `company.get_filings()`                                       |
+| Get company filings by form              | `company.get_filings(form="10-K")`                            |
+| Get a company filing by accession_number | `company.get_filing(accession_number="0000320193-21-000139")` |
+| Get the company's financials             | `company.financials`                                          |
+| Get the company's balance sheet          | `company.financials.balance_sheet`                            |
+| Get the company's cash flow statement    | `company.financials.cash_flow_statement`                      |
+
+# Installation
+
+```console
+pip install edgartools
+```
+
+# Usage
+
+
+## Set your Edgar user identity
+
+Before you can access the SEC Edgar API you need to set the identity that you will use to access Edgar.
+This is usually your name and email, or a company name and email.
+```bash
+Sample Company Name AdminContact@<sample company domain>.com
+```
+
+The user identity is sent in the User-Agent string and the Edgar API will refuse to respond to your request without it.
+
+EdgarTools will look for an environment variable called `EDGAR_IDENTITY` and use that in each request.
+So, you need to set this environment variable before using it.
+
+### Setting EDGAR_IDENTITY in Linux/Mac
+```bash
+export EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com"
+```
+
+### Setting EDGAR_IDENTITY in Windows Powershell
+```bash
+ $Env:EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com"
+```
+Alternatively, you can call `set_identity` which does the same thing.
+
+```python
+from edgar import set_identity
+set_identity("Michael Mccallum mcalum@gmail.com")
+```
+For more detail see https://www.sec.gov/os/accessing-edgar-data
+
+## Usage
+
+### Importing edgar
+
+```python
+from edgar import *
+```
+
+### Getting filings
+```python
+
+# Get filings for the current year and quarter
+filings = get_filings() 
+
+# Get filings for 2022
+filings = get_filings(2022)                 # OR filings = get_filings(year=2022)
+
+# Get filings for 2022 quarter 4
+filings = get_filings(2022, 4)              # OR filings = get_filings(year=2022, quarter=4)
+
+# Get filings for 2020, 2021 and 2022
+filings = get_filings([2020, 2021, 2022])   # OR filings = get_filings(year=range(2020, 2023))
+
+# Get filings for 2020 quarters 1 and 2
+filings = get_filings(2020, quarter=[1,2])
+```
+![Get filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/get_filings.jpg)
+
+
+
+### Filtering filings
+
+```python
+# Filter for form D
+filings.filter(form="D")
+
+# Filter for form 10-K and 10-Q 
+filings.filter(form=["10-K", "10-Q"])
+
+# When you filter by form e.g. "D" it includes amendments e.g. "D\A". You can omit amendments
+filings.filter(form="D", amendments=False)
+
+# Filter by filing_date. date and filing_date mean the same thing
+# Get all filings on 2023-02-23
+filings.filter(date="2023-02-23")                      
+# OR
+filings.filter(filing_date="2023-02-23")
+
+# Filter to get all filings between 2023-01-23 and 2023-02-23     
+filings.filter(date="2023-01-23:2023-02-23")
+
+# Filter to get all filings since 2023-01-23   
+filings.filter(date="2023-01-23")
+
+# Filter to get all filings before 2023-02-23     
+filings.filter(date=":2023-02-23")
+```
+
+### Combining getting and filtering
+```python
+get_filings(2022, form="D")
+```
+
+### Convert the filings to a pandas dataframe
+
+The filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get the data as a pandas dataframe using
+`to_pandas`
+```python
+df = filings.to_pandas()
+```
+
+
+## Navigating filings
+
+The Filings object allows you to navigate through filings using `filings.next()` and `filings.prev()`. 
+This shows you pages of the data - the page size is about 50. 
+
+```python
+# To see the next page of data
+filings.next()
+
+# To see the previous page
+filings.prev()
+
+# To see the current page
+filings.current()
+```
+
+![Get next filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filings_next.jpg)
+
+## Getting the latest filings
+
+You can get the latest **n** filings by filing_date from a filings using `filings.latest()`.
+
+If you provide the parameter `n` it will return the latest `n` filings.
+
+```python
+filing = filings.latest(n=5)
+filing
+```
+![Latest filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filings.jpg)
+
+
+If you omit this parameter, or set `n=1` it will return a single `Filings object.
+
+```python
+filing = filings.latest()
+filing
+```
+![Latest filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filing.jpg)
+
+
+## Filtering filings
+
+You can filter the filings object using te `filter()` function. This allows you to filter
+by filing date, or by form.
+
+### Filtering filings by date
+
+To filter by filing date specify the filing date in **YYYY-MM-DD** format e.g. **2022-01-24**
+(Note the parameters `date` and `filing_date` are equivalent aliases for each other)
+```python
+filings.filter(date="2021-01-24") # or filings.filter(filing_date="2021-01-24")
+```
+You can specify a filing date range using the colon
+
+```python
+filings.filter(date="2021-01-12:2021-02-28") 
+```
+To filter by dates before a specified date use `:YYYY-MM-DD'
+
+```python
+filings.filter(date=":2021-02-28") 
+```
+
+To filter by dates after a specified date use `YYYY-MM-DD:'
+
+```python
+filings.filter(date="2021-02-28:") 
+```
+
+### Filtering filings by form
+
+You can filter filings by form using the `form` parameter. 
+
+```python
+filings.filter(form="10-K") 
+```
+
+To filter by form e.g. **10-K** and include form amendments use `amendments = True`. 
+
+```python
+filings.filter(form="10-K", amendments=True) 
+```
+![Filter with amendments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filter_amendments.jpg)
+
+## Working with a single filing
+
+You can get a single filing from the filings using the bracket operator `[]`, 
+specifying the index of the filing. The index is the value displayed in the leftmost
+position in the filings table. For example, to get the **10-Q** for **Costco** in the table above
+use `filings[3]`
+
+```python
+filing = filings[3]
+```
+
+![Costco 10Q filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/costco_10Q.jpg)
+
+### View the filing homepage
+You can view the filing homepage in the terminal using `filing.homepage`
+
+This gives you access to the `FilingHomepage` class that you can use to list all the documents
+and datafiles on the filing.
+
+```python
+filing.homepage
+```
+![Filing homepage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_homepage.jpg)
+
+### Open a filing
+
+You can open the filing in your browser using `filing.open()`. This will work on environments with access to the browser, 
+will probably not work on a remote server.
+```python
+filing.open()
+```
+
+### Open the Filing Homepage
+You can open the filing homepage in the browser using `filing.homepage.open()`.
+```python
+filing.homepage.open()
+```
+
+### View the filing as Markdown
+You can view the filing's HTML content as markdown in the console using `view()`. It works for all filing types
+but can be a little slow for filings with large HTML files
+```python
+filing.view()
+```
+
+### Get the filing's html
+You can get the html content of the filing using`.html()`
+```python
+filing.html()
+```
+
+### Get the filing's html as Markdown
+You can get the html content as markdown using`.markdown()`
+```python
+filing.markdown()
+```
+
+## Viewing and downloading attachments
+
+Every filing has a list of attachments. You can view the attachments using `filing.attachments`
+
+```python
+# View the attachments
+filing.attachments
+```
+![Filing attachments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_attachments.png)
+
+You can access each attachment using the bracket operator `[]` and the index of the attachment.
+    
+```python
+# Get the first attachment
+attachment = filing.attachments[0]
+```
+
+![Filing attachments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_attachment.png)
+
+You can download the attachment using `attachment.download()`. This will download the attachment to string or bytes in memory. 
+
+## Automatic parsing of filing data
+
+Now the reason you may want to download attachments is to get information contained in data files.
+For example, **13F-HR** filings have attached infotable.xml files containing data from the holding report for that filing.
+
+Fortunately, the library handles this for you. If you call `filing.obj()` it will automatically download and parse the data files
+into a data object, for several different form types. Currently, the following forms are supported:
+
+| Form                       | Data Object            | Description                           |
+|----------------------------|------------------------|---------------------------------------|
+| 10-K                       | `TenK`                 | Annual report                         |
+| 10-Q                       | `TenQ`                 | Quarterly report                      |
+| 8-K                        | `EightK`               | Current report                        |
+| MA-I                       | `MunicipalAdvisorForm` | Municipal advisor initial filing      |
+| Form 144                   | `Form144`              | Notice of proposed sale of securities |
+| D                          | `Offering`             | Offerings                             |
+| 3,4,5                      | `Ownership`            | Ownership reports                     |
+| 13F-HR                     | `ThirteenF`             | 13F Holdings Report                   |
+| NPORT-P                    | `FundReport`           | Fund Report                           |
+| EFFECT                     | `Effect`               | Notice of Effectiveness               |
+| And other filing with XBRL | `FilingXbrl`            ||
+
+For example, to get the data object for a **13F-HR** filing you can do the following:
+
+```python
+filings = get_filings(form="13F-HR")
+filing = filings[0]
+thirteenf = filing.obj()
+```
+
+![Filing attachments](images/thirteenF.png)
+
+If you call `obj()` on a filing that does not have a data file, then it will return `None`.
+
+
+## Working with XBRL filings
+
+Some filings are in **XBRL (eXtensible Business Markup Language)** format. 
+These are mainly the newer filings, as the SEC has started requiring this for newer filings.
+
+If a filing is in XBRL format then it opens up a lot more ways to get structured data about that specific filing and also 
+about the company referred to in that filing.
+
+The `Filing` class has an `xbrl` function that will download, parse and structure the filing's XBRL document if one exists.
+If it does not exist, then `filing.xbrl()` will return `None`.
+
+The function `filing.xbrl()` returns a `FilingXbrl` instance, which wraps the data, and provides convenient
+ways of working with the xbrl data.
+
+
+```python
+filing_xbrl = filing.xbrl()
+```
+
+![Filing homapage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/10Q_xbrl.jpg)
+
+
+## Using the Company API
+
+With the company API you find a company using the **cik** or **ticker**. 
+From the company you can access all their historical **filings**,
+and a dataset of the company **facts**.
+The SEC's company API also supplies a lot more details about a company including industry, the SEC filer type,
+the mailing and business address and much more.
+
+### Find a company using the cik
+The **cik** is the id that uniquely identifies a company at the SEC.
+It is a number, but is sometimes shown in SEC Edgar resources as a string padded with leading zero's.
+For the edgar client API, just use the numbers and omit the leading zeroes.
+
+```python
+company = Company(1324424)
+```
+![expe](https://raw.githubusercontent.com/dgunning/edgartools/main/images/expe.png)
+
+
+
+### Find a company using ticker
+
+You can get a company using a ticker e.g. **SNOW**. This will do a lookup for the company cik using the ticker, then load the company using the cik.
+This makes it two calls versus one for the cik company lookup, but is sometimes more convenient since tickers are easier to remember that ciks.
+
+Note that some companies have multiple tickers, so you technically cannot get SEC filings for a ticker.
+You instead get the SEC filings for the company to which the ticker belongs.
+
+The ticker is case-insensitive so you can use `Company("snow")`
+or `Company("SNOW")`
+```python
+snow = Company("snow")
+```
+
+![snow](https://raw.githubusercontent.com/dgunning/edgartools/main/images/snow.jpg)
+### 
+
+
+```python
+Company(1832950)
+```
+
+### Get filings for a company
+To get the company's filings use `get_filings()`. This gets all the company's filings that are available from the Edgar submissions endpoint.
+
+```python
+company.get_filings()
+```
+### Filtering filings
+You can filter the company filings using a number of different parameters.
+
+```python
+class CompanyFilings:
+    
+    ...
+    
+    def get_filings(self,
+                    *,
+                    form: str | List = None,
+                    accession_number: str | List = None,
+                    file_number: str | List = None,
+                    is_xbrl: bool = None,
+                    is_inline_xbrl: bool = None
+                    ):
+        """
+        Get the company's filings and optionally filter by multiple criteria
+        :param form: The form as a string e.g. '10-K' or List of strings ['10-Q', '10-K']
+        :param accession_number: The accession number that uniquely identifies an SEC filing e.g. 0001640147-22-000100
+        :param file_number: The file number e.g. 001-39504
+        :param is_xbrl: Whether the filing is xbrl
+        :param is_inline_xbrl: Whether the filing is inline_xbrl
+        :return: The CompanyFiling instance with the filings that match the filters
+        """
+```
+
+
+#### The CompanyFilings class
+The result of `get_filings()` is a `CompanyFilings` class. This class contains a pyarrow table with the filings
+and provides convenient functions for working with filings.
+You can access the underlying pyarrow `Table` using the `.data` property
+
+```python
+filings = company.get_filings()
+
+# Get the underlying Table
+data: pa.Table = filings.data
+```
+
+#### Get a filing by index
+To access a filing in the CompanyFilings use the bracket `[]` notation e.g. `filings[2]`
+```python
+filings[2]
+```
+
+#### Get the latest filing
+
+The `CompanyFilings` class has a `latest` function that will return the latest `Filing`. 
+So, to get the latest **10-Q** filing, you do the following
+```python
+# Latest filing makes sense if you filter by form  type e.g. 10-Q
+snow_10Qs = snow.get_filings(form='10-Q')
+latest_10Q = snow_10Qs.latest()
+
+# Or chain the function calls
+snow.get_filings(form='10-Q').latest()
+```
+
+
+### Get company facts
+
+Facts are an interesting and important dataset about a company accumlated from data the company provides to the SEC.
+Company facts are available for a company on the Company Facts`f"https://data.sec.gov/api/xbrl/companyfacts/CIK{cik:010}.json"`
+It is a JSON endpoint and `edgartools` parses the JSON into a structured dataset - a `pyarrow.Table`.
+
+#### Getting facts for a company
+To get company facts, first get the company, then call `company.get_facts()`
+```python
+company = Company("SNOW")
+company_facts = company.get_facts()
+```
+The result is a `CompanyFacts` object which wraps the underlying facts and provides convenient ways of working
+with the facts data. To get access to the underyling data use the `facts` property.
+
+You can get the facts as a pandas dataframe by calling `to_pandas`
+
+```python
+df = company_facts.to_pandas()
+```
+
+Facts differ among companies. To see what facts are available you can use the `facts_meta` property.
+
+
+# Contributing
+
+Contributions are welcome! We would love to hear your thoughts on how this library could be better at working with SEC Edgar.
+
+## Reporting Issues
+We use GitHub issues to track public bugs. 
+Report a bug by [opening a new issue](https://github.com/dgunning/edgartools/issues); it's that easy!
+
+## Making code changes
+- Fork the repo and create your branch from master.
+- If you've added code that should be tested, add tests.
+- If you've changed APIs, update the documentation.
+- Ensure the test suite passes.
+- Make sure your code lints.
+- Issue that pull request!
+
+
+
+# License
+
+`edgartools` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Contact
+
 [LinkedIn](https://www.linkedin.com/in/dwight-gunning-860124/)
```

#### html2text {}

```diff
@@ -1,9 +1,28 @@
- ![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/
-main/images/edgar-tools.png) [![PyPI - Version](https://img.shields.io/pypi/v/
+Metadata-Version: 2.1 Name: edgartools Version: 2.0.2 Summary: One of the
+nicest looking EDGAR libraries out there Project-URL: Documentation, https://
+dgunning.github.io/edgartools/ Project-URL: Issues, https://github.com/
+dgunning/edgartools/issues Project-URL: Source, https://github.com/dgunning/
+edgartools Author-email: Dwight Gunning
+gmail.com> License-File: LICENSE.txt Keywords:
+company,edgar,filings,finance,financial,python,reports,sec Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8 Requires-
+Dist: beautifulsoup4>=4.10.0 Requires-Dist: charset-normalizer>=2.1.1 Requires-
+Dist: fastcore>=1.5.20 Requires-Dist: httpx>=0.23.1 Requires-Dist:
+humanize>=4.0.0 Requires-Dist: lxml>=4.4 Requires-Dist: markdownify>0.11.0
+Requires-Dist: pandas>=1.3.0 Requires-Dist: pyarrow>=11.0.0 Requires-Dist:
+rank-bm25==0.2.1 Requires-Dist: retry>=0.9.2 Requires-Dist: rich>=13.0.0
+Requires-Dist: textdistance>=4.5.0 Description-Content-Type: text/markdown !
+[edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/main/
+images/edgar-tools.png) [![PyPI - Version](https://img.shields.io/pypi/v/
 edgartools.svg)](https://pypi.org/project/edgartools) ![GitHub last commit]
 (https://img.shields.io/github/last-commit/dgunning/edgartools) ![GitHub
 Workflow Status](https://img.shields.io/github/actions/workflow/status/
 dgunning/edgartools/python-hatch-workflow.yml) [![CodeFactor](https://
 www.codefactor.io/repository/github/dgunning/edgartools/badge)](https://
 www.codefactor.io/repository/github/dgunning/edgartools) [![Hatch project]
 (https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://
@@ -17,100 +36,141 @@
           o Set_your_Edgar_user_identity
           o Getting_Filings
           o Using_the_Company_API
    4. Contributing
    5. License
    6. Contact
  # About the project **`edgartools`** is one of the nicest looking EDGAR
-libraries out there. You can query, filter and select any filing since 1994 and
-view the filing's html, text, xml or structured data. ## Demo #### Show 20 10-
-K filings for the 2nd quarter of 2023 and open the first in the browser
-```python from edgar import * # Get 10-K filings for the second quarter of 2023
-ten_k_filings = get_filings(2023, 2, form="10-K") # Get the latest 20 filings
-from the list latest_ten_k_filings = filings.latest(20) # Open the 1st filing
-in the browser latest_ten_k_filings[0].open() ``` ![10 K Filings](https://
-raw.githubusercontent.com/dgunning/edgartools/main/images/
-latest_10K_filings.png) ## Features ### Start with filings, filter down to a
-filing - View filings since 1994 to today - Filter filings by **form e.g.
-10K**, **filing date** etc. - Page through filings using **next()** and **prev
-()** - Select and view a filing in the terminal, or open in the browser -
-Download any file from any filing - Parse XML for **Offering, Ownership** and
-other filing types - Automatically parse a filing's XBRL into a pandas
-dataframe ### Start with a Company, get their filings and Facts - Search for
-company by ticker or CIK - View a company's filings - Page through filings
-using **next()** and **prev()** - Get a company **facts** e.g.
-**CommonSharesOutstanding** as a dataframe # Installation ```console pip
-install edgartools ``` # Usage ## Set your Edgar user identity Before you can
-access the SEC Edgar API you need to set the identity that you will use to
-access Edgar. This is usually your name and email, or a company name and email.
-```bash Sample Company Name AdminContact@.com ``` The user identity is sent in
-the User-Agent string and the Edgar API will refuse to respond to your request
-without it. EdgarTools will look for an environment variable called
-`EDGAR_IDENTITY` and use that in each request. So, you need to set this
-environment variable before using it. ### Setting EDGAR_IDENTITY in Linux/Mac
-```bash export EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com" ``` ###
-Setting EDGAR_IDENTITY in Windows Powershell ```bash $Env:
-EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com" ``` Alternatively, you can
-call `set_identity` which does the same thing. ```python from edgar import
-set_identity set_identity("Michael Mccallum mcalum@gmail.com") ``` For more
-detail see https://www.sec.gov/os/accessing-edgar-data ## Usage ### Importing
-edgar ```python from edgar import * ``` ### Getting filings ```python # Get
-filings for the current year and quarter filings = get_filings() # Get filings
-for 2022 filings = get_filings(2022) # OR filings = get_filings(year=2022) #
-Get filings for 2022 quarter 4 filings = get_filings(2022, 4) # OR filings =
-get_filings(year=2022, quarter=4) # Get filings for 2020, 2021 and 2022 filings
-= get_filings([2020, 2021, 2022]) # OR filings = get_filings(year=range(2020,
-2023)) # Get filings for 2020 quarters 1 and 2 filings = get_filings(2020,
-quarter=[1,2]) ``` ![Get filings](https://raw.githubusercontent.com/dgunning/
-edgartools/main/images/get_filings.jpg) ### Filtering filings ```python #
-Filter for form D filings.filter(form="D") # Filter for form 10-K and 10-
-Q filings.filter(form=["10-K", "10-Q"]) # When you filter by form e.g. "D" it
-includes amendments e.g. "D\A". You can omit amendments filings.filter
-(form="D", amendments=False) # Filter by filing_date. date and filing_date mean
-the same thing # Get all filings on 2023-02-23 filings.filter(date="2023-02-
-23") # OR filings.filter(filing_date="2023-02-23") # Filter to get all filings
-between 2023-01-23 and 2023-02-23 filings.filter(date="2023-01-23:2023-02-23")
-# Filter to get all filings since 2023-01-23 filings.filter(date="2023-01-23")
-# Filter to get all filings before 2023-02-23 filings.filter(date=":2023-02-
-23") ``` ### Combining getting and filtering ```python get_filings(2022,
-form="D") ``` ### Convert the filings to a pandas dataframe The filings data is
-stored in the `Filings` class as a `pyarrow.Table`. You can get the data as a
-pandas dataframe using `to_pandas` ```python df = filings.to_pandas() ``` ##
-Navigating filings The Filings object allows you to navigate through filings
-using `filings.next()` and `filings.prev()`. This shows you pages of the data -
-the page size is about 50. ```python # To see the next page of data
-filings.next() # To see the previous page filings.prev() # To see the current
-page filings.current() ``` ![Get next filings](https://
-raw.githubusercontent.com/dgunning/edgartools/main/images/filings_next.jpg) ##
-Getting the latest filings You can get the latest **n** filings by filing_date
-from a filings using `filings.latest()`. If you provide the parameter `n` it
-will return the latest `n` filings. ```python filing = filings.latest(n=5)
-filing ``` ![Latest filings](https://raw.githubusercontent.com/dgunning/
-edgartools/main/images/latest_filings.jpg) If you omit this parameter, or set
-`n=1` it will return a single `Filings object. ```python filing =
-filings.latest() filing ``` ![Latest filing](https://raw.githubusercontent.com/
-dgunning/edgartools/main/images/latest_filing.jpg) ## Filtering filings You can
-filter the filings object using te `filter()` function. This allows you to
-filter by filing date, or by form. ### Filtering filings by date To filter by
-filing date specify the filing date in **YYYY-MM-DD** format e.g. **2022-01-
-24** (Note the parameters `date` and `filing_date` are equivalent aliases for
-each other) ```python filings.filter(date="2021-01-24") # or filings.filter
-(filing_date="2021-01-24") ``` You can specify a filing date range using the
-colon ```python filings.filter(date="2021-01-12:2021-02-28") ``` To filter by
-dates before a specified date use `:YYYY-MM-DD' ```python filings.filter
-(date=":2021-02-28") ``` To filter by dates after a specified date use `YYYY-
-MM-DD:' ```python filings.filter(date="2021-02-28:") ``` ### Filtering filings
-by form You can filter filings by form using the `form` parameter. ```python
-filings.filter(form="10-K") ``` To filter by form e.g. **10-K** and include
-form amendments use `amendments = True`. ```python filings.filter(form="10-K",
-amendments=True) ``` ![Filter with amendments](https://
-raw.githubusercontent.com/dgunning/edgartools/main/images/
-filter_amendments.jpg) ## Getting a single filing You can get a single filing
-from the filings using the bracket operator `[]`, specifying the index of the
-filing. The index is the value displayed in the leftmost position in the
+libraries out there. It is also powerful and easy to use. You can query, filter
+and select any filing since 1994 and view the filing's html, text, xml or
+structured data. ## Demo #### Show 20 10-K filings for the 2nd quarter of 2023
+and open the first in the browser ```python from edgar import * # Get 10-
+K filings for the second quarter of 2023 ten_k_filings = get_filings(2023, 2,
+form="10-K") # Get the latest 20 filings by date latest_ten_k_filings =
+filings.latest(20) # Show the first filing latest_ten_k_filings[0] ``` ![10 K
+Filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/
+latest_10K_filing.png) ## Features ### Getting started | Task | Code | |-------
+-------------------------------|-----------------------------------------------
+--------| | Set your EDGAR identity in Linux/Mac | `export
+EDGAR_IDENTITY="First Last email@domain.com"` | | Set your EDGAR identity in
+Windows | `set EDGAR_IDENTITY="First Last email@domain.com"` | | Set identity
+in Windows Powershell | `$env:EDGAR_IDENTITY="First Last email@domain.com"` | |
+Set identity in Python | `set_identity("First Last email@domain.com")` | |
+Importing the library | `from edgar import *` | ### Working with filings | Task
+| Code | |------------------------------------|--------------------------------
+---------------| | Get filings for the year to date | `filings = get_filings()`
+| | Get only xbrl filings | `filings = get_filings(index="xbrl")` | | Get
+filings for a specific year | `filings = get_filings(2020)` | | Get filings for
+a specific quarter | `filings = get_filings(2020, 1)` | | Get filings for
+multiple years | `filings = get_filings([2020, 2021])` | | Get filigs for a
+range of years | `filings = get_filings(year=range(2010, 2020)` | | Get filings
+for a specific form | `filings = get_filings(form="10-K")` | | Get filings for
+a list of forms | `filings = get_filings(form=["10-K", "10-Q"])` | | Show the
+next page of filings | `filings.next()` | | Show the previous page of filings |
+`filings.prev()` | | Get the first n filings | `filings.head(20)` | | Get the
+last n filings | `filings.tail(20)` | | Get the latest n filings by date |
+`filings.latest(20)` | | Get a random sample of the filings | `filings.sample
+(20)` | | Filter filings on a date | `filings = filings.filter(date="2020-01-
+01")` | | Filter filings between dates | `filings.filter(date="2020-01-01:2020-
+03-01")` | | Filter filings before a date | `filings.filter(date=":2020-03-
+01")` | | Filter filings after a date | `filings.filter(date="2020-03-01:")` |
+| Get filings as a pandas dataframe | `filings.to_pandas()` | ### Working with
+a filing | Task | Code | |-------------------------------------------|---------
+--------------------------------------------------| | Get a single filing |
+`filing = filings[3]` | | Get a filing by accession number | `filing =
+get_by_accession_number("0000320193-20-34576")` | | Get the filing homepage |
+`filing.homepage` | | Open a filing in the browser | `filing.open()` | | Open
+the filing homepage in the browser | `filing.homepage.open()` | | View the
+filing in the terminal | `filing.view()` | | Get the html of the filing
+document | `filing.html()` | | Get the XBRL of the filing document |
+`filing.xbrl()` | | Get the filing document as markdown | `filing.markdown()` |
+| Get the full submission text of a filing | `filing.text()` | | Get and parse
+the data object of a filing | `filing.obj()` | | Get the filing attachments |
+`filing.attachments` | | Get a single attachment | `attachment =
+filing.attachments[0]` | | Open an attachment in the browser | `attachment.open
+()` | | Download an attachment | `content = attachment.download()` | ###
+Working with a company | Task | Code | |---------------------------------------
+---|---------------------------------------------------------------| | Get a
+company by ticker | `company = Company("AAPL")` | | Get a company by CIK |
+`company = Company("0000320193")` | | Get company facts | `company.get_facts()`
+| | Get company facts as a pandas dataframe | `company.get_facts().to_pandas()`
+| | Get company filings | `company.get_filings()` | | Get company filings by
+form | `company.get_filings(form="10-K")` | | Get a company filing by
+accession_number | `company.get_filing(accession_number="0000320193-21-
+000139")` | | Get the company's financials | `company.financials` | | Get the
+company's balance sheet | `company.financials.balance_sheet` | | Get the
+company's cash flow statement | `company.financials.cash_flow_statement` | #
+Installation ```console pip install edgartools ``` # Usage ## Set your Edgar
+user identity Before you can access the SEC Edgar API you need to set the
+identity that you will use to access Edgar. This is usually your name and
+email, or a company name and email. ```bash Sample Company Name
+AdminContact@.com ``` The user identity is sent in the User-Agent string and
+the Edgar API will refuse to respond to your request without it. EdgarTools
+will look for an environment variable called `EDGAR_IDENTITY` and use that in
+each request. So, you need to set this environment variable before using it.
+### Setting EDGAR_IDENTITY in Linux/Mac ```bash export EDGAR_IDENTITY="Michael
+Mccallum mcalum@gmail.com" ``` ### Setting EDGAR_IDENTITY in Windows Powershell
+```bash $Env:EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com" ```
+Alternatively, you can call `set_identity` which does the same thing. ```python
+from edgar import set_identity set_identity("Michael Mccallum
+mcalum@gmail.com") ``` For more detail see https://www.sec.gov/os/accessing-
+edgar-data ## Usage ### Importing edgar ```python from edgar import * ``` ###
+Getting filings ```python # Get filings for the current year and quarter
+filings = get_filings() # Get filings for 2022 filings = get_filings(2022) # OR
+filings = get_filings(year=2022) # Get filings for 2022 quarter 4 filings =
+get_filings(2022, 4) # OR filings = get_filings(year=2022, quarter=4) # Get
+filings for 2020, 2021 and 2022 filings = get_filings([2020, 2021, 2022]) # OR
+filings = get_filings(year=range(2020, 2023)) # Get filings for 2020 quarters 1
+and 2 filings = get_filings(2020, quarter=[1,2]) ``` ![Get filings](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/get_filings.jpg) ###
+Filtering filings ```python # Filter for form D filings.filter(form="D") #
+Filter for form 10-K and 10-Q filings.filter(form=["10-K", "10-Q"]) # When you
+filter by form e.g. "D" it includes amendments e.g. "D\A". You can omit
+amendments filings.filter(form="D", amendments=False) # Filter by filing_date.
+date and filing_date mean the same thing # Get all filings on 2023-02-23
+filings.filter(date="2023-02-23") # OR filings.filter(filing_date="2023-02-23")
+# Filter to get all filings between 2023-01-23 and 2023-02-23 filings.filter
+(date="2023-01-23:2023-02-23") # Filter to get all filings since 2023-01-23
+filings.filter(date="2023-01-23") # Filter to get all filings before 2023-02-23
+filings.filter(date=":2023-02-23") ``` ### Combining getting and filtering
+```python get_filings(2022, form="D") ``` ### Convert the filings to a pandas
+dataframe The filings data is stored in the `Filings` class as a
+`pyarrow.Table`. You can get the data as a pandas dataframe using `to_pandas`
+```python df = filings.to_pandas() ``` ## Navigating filings The Filings object
+allows you to navigate through filings using `filings.next()` and `filings.prev
+()`. This shows you pages of the data - the page size is about 50. ```python #
+To see the next page of data filings.next() # To see the previous page
+filings.prev() # To see the current page filings.current() ``` ![Get next
+filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/
+filings_next.jpg) ## Getting the latest filings You can get the latest **n**
+filings by filing_date from a filings using `filings.latest()`. If you provide
+the parameter `n` it will return the latest `n` filings. ```python filing =
+filings.latest(n=5) filing ``` ![Latest filings](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filings.jpg)
+If you omit this parameter, or set `n=1` it will return a single `Filings
+object. ```python filing = filings.latest() filing ``` ![Latest filing](https:/
+/raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filing.jpg)
+## Filtering filings You can filter the filings object using te `filter()`
+function. This allows you to filter by filing date, or by form. ### Filtering
+filings by date To filter by filing date specify the filing date in **YYYY-MM-
+DD** format e.g. **2022-01-24** (Note the parameters `date` and `filing_date`
+are equivalent aliases for each other) ```python filings.filter(date="2021-01-
+24") # or filings.filter(filing_date="2021-01-24") ``` You can specify a filing
+date range using the colon ```python filings.filter(date="2021-01-12:2021-02-
+28") ``` To filter by dates before a specified date use `:YYYY-MM-DD' ```python
+filings.filter(date=":2021-02-28") ``` To filter by dates after a specified
+date use `YYYY-MM-DD:' ```python filings.filter(date="2021-02-28:") ``` ###
+Filtering filings by form You can filter filings by form using the `form`
+parameter. ```python filings.filter(form="10-K") ``` To filter by form e.g.
+**10-K** and include form amendments use `amendments = True`. ```python
+filings.filter(form="10-K", amendments=True) ``` ![Filter with amendments]
+(https://raw.githubusercontent.com/dgunning/edgartools/main/images/
+filter_amendments.jpg) ## Working with a single filing You can get a single
+filing from the filings using the bracket operator `[]`, specifying the index
+of the filing. The index is the value displayed in the leftmost position in the
 filings table. For example, to get the **10-Q** for **Costco** in the table
 above use `filings[3]` ```python filing = filings[3] ``` ![Costco 10Q filing]
 (https://raw.githubusercontent.com/dgunning/edgartools/main/images/
 costco_10Q.jpg) ### View the filing homepage You can view the filing homepage
 in the terminal using `filing.homepage` This gives you access to the
 `FilingHomepage` class that you can use to list all the documents and datafiles
 on the filing. ```python filing.homepage ``` ![Filing homepage](https://
```

### Comparing `edgartools-2.0.1/pyproject.toml` & `edgartools-2.0.2/pyproject.toml`

 * *Files identical despite different names*

