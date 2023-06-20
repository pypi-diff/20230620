# Comparing `tmp/feriados_brasileiros-0.0.2.tar.gz` & `tmp/feriados_brasileiros-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feriados_brasileiros-0.0.2.tar", last modified: Mon Jun 19 02:42:59 2023, max compression
+gzip compressed data, was "feriados_brasileiros-0.0.3.tar", last modified: Tue Jun 20 02:33:43 2023, max compression
```

## Comparing `feriados_brasileiros-0.0.2.tar` & `feriados_brasileiros-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/feriados_brasileiros/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/datas.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:33:43.377911 feriados_brasileiros-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-20 02:33:43.377911 feriados_brasileiros-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:33:43.377911 feriados_brasileiros-0.0.3/feriados_brasileiros/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/feriados_brasileiros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/feriados_brasileiros/datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:33:43.377911 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-20 02:33:43.000000 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 02:33:43.000000 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:33:43.000000 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:33:43.000000 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:33:43.000000 feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 02:33:43.377911 feriados_brasileiros-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:33:34.000000 feriados_brasileiros-0.0.3/setup.py
```

### Comparing `feriados_brasileiros-0.0.2/LICENSE` & `feriados_brasileiros-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.2/MANIFEST.in` & `feriados_brasileiros-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.2/PKG-INFO` & `feriados_brasileiros-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: feriados_brasileiros
-Version: 0.0.2
-Summary: Feriados Brasileiros
-Home-page: https://github.com/michelmetran/feriados
-Author: Michel Metran
-Author-email: michelmetran@gmail.com
-Keywords: python,dados espaciais,geoprocessamento
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Portuguese
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Feriados Brasileiros
 
 [PyPI](https://pypi.org/project/feriados-brasileiros) | [GitHub](https://github.com/michelmetran/feriados)
 
 <br>
 
 > _Adoro um feriado! Quem não gosta?!_
@@ -43,75 +26,100 @@
 
 ---
 
 ## Como Usar?!
 
 A maneira mais simples é obter todos os feriados para um determinado ano. Dessa forma os atributos serão definidos por padrão.
 
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados
+```
+
+<br>
+
+---
+
+## Detalhes
+
+É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos para cada um dos feriados.
+
 Dentre os atributos existentes estão:
 
-- `nome`: Nome do Feriado;
-- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente;
+- `nome_alternativo`: Nome do Feriado;
+- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
-from feriados_brasileiros import Feriados
+from feriados_brasileiros import datas
 
-# Lista Todos dos Feriados de um determinado Ano
+# Adiciona apenas um feriado de um determinado ano
 feriados = Feriados(ano=2023)
+feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
+feriados
+```
+
+<br>
+
+---
+
+## Remoção
+
+É possível remover feriados específicos, após ter adicionado todos!.
+
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
 feriados.add_all()
+feriados.remove('Domingo de Ramos')
+feriados.remove('Endoenças')
+feriados
 ```
 
 <br>
 
 ---
 
-## Detalhes
+## _Custom_
 
-É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos (`nome`, `feriado`, `obs`) para cada um dos feriados.
+Também é possível adicioanr um feriado customizado.
 
 ```python
-# Lista Todos dos Feriados de um determinado Ano
-feriados = Feriados(ano=2023)
+from feriados_brasileiros import datas
 
-# Feriados Móveis
-feriados.add_carnaval_seg(nome='Segundona de Carnaval!')
-feriados.add_carnaval_ter()
-feriados.add_carnaval_qua(obs='Entrada no serviço após as 14h!')
-feriados.add_endoencas(obs='Endoenças: é feriado isso?!', feriado=False)
-feriados.add_paixao_cristo(nome='Sexta-feira Santa', obs='Paixão de Cristo')
-feriados.add_pascoa(obs='Quero chocolate!!')
-feriados.add_corpus_christ()
-
-# Feriados Fixos
-feriados.add_confraternizacao()
-feriados.add_aniversario_sao_paulo(feriado=False)
-feriados.add_tiradentes()
-feriados.add_trabalho()
-feriados.add_independencia(obs='Independência ou Morte!')
-feriados.add_padroeira()
-feriados.add_finados()
-feriados.add_proclamacao_republica(obs='Dia de ler sobre o arretado Ruy Barbosa!')
-feriados.add_consciencia_negra()
-feriados.add_vespera_natal(feriado=False)
-feriados.add_natal()
-feriados.add_reveillon(feriado=False)
+# Adiciona todos os feriados de um determinado ano, além de outras feriados customizados (municipais e estaduais, por exemplo)
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados.add_custom(
+    nome='Dia do Servidor Público',
+    mes=10,
+    dia=28,
+    feriado=True,
+    tipo='Fixo',
+)
+feriados
 ```
 
 <br>
 
 ---
 
 ## Resultados
 
 Seja qual for a opção escolhida para usar o programa, os resultados podem ser obtidos de duas formas distintas.
 
 ```python
 # Resultado em Lista
-lista_feriados = feriados.create_list()
+lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
 df = feriados.create_table()
 print(df.head())
 ```
 
@@ -127,11 +135,11 @@
 
 <br>
 
 ---
 
 ## _TODO_
 
-1. Ajustar documentação
+1. ~~Ajustar documentação~~
 2. ~~Incluir o dia da semana!~~
 3. ~~Implantar classe Calendário para pegar feriados de anos diversos~~
 4. ~~Add domingo de ramos~~
```

### Comparing `feriados_brasileiros-0.0.2/README.md` & `feriados_brasileiros-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: feriados_brasileiros
+Version: 0.0.3
+Summary: Feriados Brasileiros
+Home-page: https://github.com/michelmetran/feriados
+Author: Michel Metran
+Author-email: michelmetran@gmail.com
+Keywords: python,dados espaciais,geoprocessamento
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Portuguese
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Feriados Brasileiros
 
 [PyPI](https://pypi.org/project/feriados-brasileiros) | [GitHub](https://github.com/michelmetran/feriados)
 
 <br>
 
 > _Adoro um feriado! Quem não gosta?!_
@@ -26,75 +43,100 @@
 
 ---
 
 ## Como Usar?!
 
 A maneira mais simples é obter todos os feriados para um determinado ano. Dessa forma os atributos serão definidos por padrão.
 
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados
+```
+
+<br>
+
+---
+
+## Detalhes
+
+É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos para cada um dos feriados.
+
 Dentre os atributos existentes estão:
 
-- `nome`: Nome do Feriado;
-- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente;
+- `nome_alternativo`: Nome do Feriado;
+- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
-from feriados_brasileiros import Feriados
+from feriados_brasileiros import datas
 
-# Lista Todos dos Feriados de um determinado Ano
+# Adiciona apenas um feriado de um determinado ano
 feriados = Feriados(ano=2023)
+feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
+feriados
+```
+
+<br>
+
+---
+
+## Remoção
+
+É possível remover feriados específicos, após ter adicionado todos!.
+
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
 feriados.add_all()
+feriados.remove('Domingo de Ramos')
+feriados.remove('Endoenças')
+feriados
 ```
 
 <br>
 
 ---
 
-## Detalhes
+## _Custom_
 
-É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos (`nome`, `feriado`, `obs`) para cada um dos feriados.
+Também é possível adicioanr um feriado customizado.
 
 ```python
-# Lista Todos dos Feriados de um determinado Ano
-feriados = Feriados(ano=2023)
+from feriados_brasileiros import datas
 
-# Feriados Móveis
-feriados.add_carnaval_seg(nome='Segundona de Carnaval!')
-feriados.add_carnaval_ter()
-feriados.add_carnaval_qua(obs='Entrada no serviço após as 14h!')
-feriados.add_endoencas(obs='Endoenças: é feriado isso?!', feriado=False)
-feriados.add_paixao_cristo(nome='Sexta-feira Santa', obs='Paixão de Cristo')
-feriados.add_pascoa(obs='Quero chocolate!!')
-feriados.add_corpus_christ()
-
-# Feriados Fixos
-feriados.add_confraternizacao()
-feriados.add_aniversario_sao_paulo(feriado=False)
-feriados.add_tiradentes()
-feriados.add_trabalho()
-feriados.add_independencia(obs='Independência ou Morte!')
-feriados.add_padroeira()
-feriados.add_finados()
-feriados.add_proclamacao_republica(obs='Dia de ler sobre o arretado Ruy Barbosa!')
-feriados.add_consciencia_negra()
-feriados.add_vespera_natal(feriado=False)
-feriados.add_natal()
-feriados.add_reveillon(feriado=False)
+# Adiciona todos os feriados de um determinado ano, além de outras feriados customizados (municipais e estaduais, por exemplo)
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados.add_custom(
+    nome='Dia do Servidor Público',
+    mes=10,
+    dia=28,
+    feriado=True,
+    tipo='Fixo',
+)
+feriados
 ```
 
 <br>
 
 ---
 
 ## Resultados
 
 Seja qual for a opção escolhida para usar o programa, os resultados podem ser obtidos de duas formas distintas.
 
 ```python
 # Resultado em Lista
-lista_feriados = feriados.create_list()
+lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
 df = feriados.create_table()
 print(df.head())
 ```
 
@@ -110,11 +152,11 @@
 
 <br>
 
 ---
 
 ## _TODO_
 
-1. Ajustar documentação
+1. ~~Ajustar documentação~~
 2. ~~Incluir o dia da semana!~~
 3. ~~Implantar classe Calendário para pegar feriados de anos diversos~~
 4. ~~Add domingo de ramos~~
```

### Comparing `feriados_brasileiros-0.0.2/feriados_brasileiros/datas.py` & `feriados_brasileiros-0.0.3/feriados_brasileiros/datas.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,149 +37,149 @@
         self.dict_tipo = {
             # Móvel
             'Carnaval (seg)': {
                 'data': dt_carnaval_seg,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Carnaval (ter)': {
                 'data': dt_carnaval_ter,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Carnaval (qua)': {
                 'data': dt_carnaval_qua,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Domingo de Ramos': {
                 'data': dt_dom_ramos,
                 'nome_alternativo': None,
                 'feriado': False,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Páscoa': {
                 'data': dt_pascoa,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Sexta-feira Santa': {
                 'data': dt_paixao_cristo,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Endoenças': {
                 'data': dt_endoencas,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             'Corpus Christ': {
                 'data': dt_corpus_christ,
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Móvel',
-                'obs': None,
+                'obs': '',
             },
             # Fixo
             'Confraternização Universal': {
                 'data': date(self.ano, 1, 1),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Aniversário da Cidade de São Paulo': {
                 'data': date(self.ano, 1, 25),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Tiradentes': {
                 'data': date(self.ano, 4, 21),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Dia do Trabalho': {
                 'data': date(self.ano, 5, 1),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Independência do Brasil': {
                 'data': date(self.ano, 9, 7),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Dia de Nossa Senhora Aparecida': {
                 'data': date(self.ano, 10, 12),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Dia de Finados': {
                 'data': date(self.ano, 11, 2),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Proclamação da República': {
                 'data': date(self.ano, 11, 15),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Dia da Consciência Negra': {
                 'data': date(self.ano, 11, 20),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Véspera de Natal': {
                 'data': date(self.ano, 12, 24),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Natal': {
                 'data': date(self.ano, 12, 25),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
             'Reveillon': {
                 'data': date(self.ano, 12, 31),
                 'nome_alternativo': None,
                 'feriado': True,
                 'tipo': 'Fixo',
-                'obs': None,
+                'obs': '',
             },
         }
         #
         self.feriados_disponiveis = list(self.dict_tipo.keys())
         self.dict_feriados_solicitados = {}
 
     def _realizar_calculo(self):
@@ -197,87 +197,31 @@
         if res > 9:
             self.dia = res - 9
             self.mes = 4
         else:
             self.dia = res + 22
             self.mes = 3
 
-    def add_all(self):
-        """
-        Adiciona todos os feriados, com as descrições,
-        observações e atributos "padrão"
-        """
-        for feriado in self.feriados_disponiveis:
-            self.add(nome=feriado)
-
-    def create_table(self):
-        """
-        Cria uma tabela de Feriados, em formato pandas,
-        contendo os feriados adicionados individualmente,
-        ou total (com o método "add_all()").
-
-        Apresenta diversas descrições e atributos que
-        podem ser customizadas caso o usuário optei por
-        adicionar os feriados individualmente.
-
-        :return: Tabela com Feriados
-        :rtype: dataframe
-        """
-        # Adjust Table
-        if len(self.dict_feriados_solicitados) == 0:
-            raise Warning('Necessário Adicionar feriados!')
-
-        dataframe = pd.DataFrame.from_dict(
-            self.dict_feriados_solicitados, orient='index'
-        )
-        # df = df[pd.notna(df['data'])]
-        dataframe = dataframe.sort_values(['data'], ascending=True)
-        dataframe['data'] = pd.to_datetime(dataframe['data'])
-        dataframe['dia_semama'] = df['data'].dt.day_name(locale='PT')
-        dataframe = dataframe.reset_index(drop=True)
-        dataframe = dataframe.rename({'nome_alternativo': 'nome'}, axis=1)
-        dataframe = dataframe[
-            ['data', 'dia_semama', 'nome', 'feriado', 'tipo', 'obs']
-        ]
-        return dataframe
-
-    def create_list(self):
-        """
-        Cria uma lista de Feriados, em formato datetime,
-        contendo os feriados adicionados individualmente,
-        ou total (com o método "all()")
-
-        :return: Lista dos Feriados
-        :rtype: list
+    def add(self, nome, nome_alternativo=None, feriado=None, obs=''):
         """
-        # Cria Tabela
-        df = self.create_table()
-        list_feriados = list(df['data'])
+        Adiciona feriado
 
-        # Results
-        list_feriados = [x for x in list_feriados if pd.notna(x)]
-        list_feriados = [datetime.date(x) for x in df['data']]
-        return list_feriados
-
-    def add(self, nome, nome_alternativo=None, feriado=None, obs=None):
+        :param nome: Nome do feriado
+        :type nome: string
+        :param nome_alternativo: Nome do feriado alternativo, caso queira ajustar o nome "padrão", defaults to None
+        :type nome_alternativo: string, optional
+        :param feriado: Define se é, ou não, feriado (True/False), defaults to None
+        :type feriado: bool, optional
+        :param obs: Acrescenta uma observação ao feriado, defaults to None
+        :type obs: string, optional
+        :raises Warning: Avalia se o feriado solicitado consta na lista dos "feriados_disponiveis"
+        :return: Retorna a data do feriado
+        :rtype: date
         """
-        _summary_
 
-        :param nome: _description_
-        :type nome: _type_
-        :param nome_alternativo: _description_, defaults to None
-        :type nome_alternativo: _type_, optional
-        :param feriado: _description_, defaults to None
-        :type feriado: _type_, optional
-        :param obs: _description_, defaults to None
-        :type obs: _type_, optional
-        :raises Warning: _description_
-        :return: _description_
-        :rtype: _type_
-        """
         if nome not in self.feriados_disponiveis:
             fer = '\n'.join(self.feriados_disponiveis)
             raise Warning(
                 f'O feriado precisa ser um dos listados abaixo\n{fer}'
             )
 
         # Pega o Tipo do Feriado no dict padrão!
@@ -306,52 +250,52 @@
         dict_temp = self.dict_feriados_solicitados
         dict_temp.update(dict_feriado)
         self.dict_feriados_solicitados = dict_temp
 
         # Results
         return self.dict_tipo[nome]['data']
 
-    def remove(self, nome):
+    def add_all(self):
         """
-        Summary
-
-        :param nome: _description_
-        :type nome: _type_
-        :raises Warning: _description_
-        :return: _description_
-        :rtype: _type_
+        Adiciona todos os feriados, com as descrições,
+        observações e atributos "padrão"
         """
-        if nome not in self.feriados_disponiveis:
-            fer = '\n'.join(self.feriados_disponiveis)
-            raise Warning(
-                f'O feriado precisa ser um dos listados abaixo\n{fer}'
-            )
-        # Feriados Solicitados
-        dict_temp = self.dict_feriados_solicitados
-        feriado_del = dict_temp.pop(nome)
-        self.dict_feriados_solicitados = dict_temp
-        return feriado_del['data']
+        for feriado in self.feriados_disponiveis:
+            self.add(nome=feriado)
 
     def add_custom(self, nome, mes, dia, feriado, tipo, obs=None):
         """
-        _summary_
-
-        :param nome: _description_
-        :type nome: _type_
-        :param data: _description_
-        :type data: _type_
-        :param feriado: _description_
-        :type feriado: _type_
-        :param tipo: _description_
-        :type tipo: _type_
-        :param obs: _description_, defaults to None
-        :type obs: _type_, optional
-        :return: _description_
-        :rtype: _type_
+        Adiciona um feriado "customizado".
+        Ideal para feriados municipais,
+        não disponíveis no atributo "feriados_disponiveis"
+
+        :param nome: Nome do feriado
+        :type nome: string
+        :param mes: Número do mês do feriado
+        :type mes: int
+        :param dia: Número do dia do feriado
+        :type dia: int
+        :param feriado: Define se é, ou não, feriado (True/False)
+        :type feriado: bool
+        :param tipo: tipo "Fixo" ou "Móvel"
+        :type tipo: string
+        :param obs: Acrescenta uma observação ao feriado, defaults to None
+        :type obs: string, optional
+        :return: Retorna a data do feriado
+        :rtype: date
         """
+        if mes not in range(1, 13):
+            raise Warning('Mês precisa ser menor que 12')
+
+        if dia not in range(1, 31):
+            raise Warning('Dia precisa ser menor que 31')
+
+        if tipo not in ['Fixo', 'Móvel']:
+            raise Warning('O feriado precisa ser do tipo "Fixo" ou "Móvel"')
+
         data = date(self.ano, mes, dia)
 
         # Cria Dicionário
         dict_feriado = {
             nome: {
                 'data': data,
                 'nome_alternativo': nome,
@@ -363,33 +307,127 @@
 
         # Feriados Solicitados
         dict_temp = self.dict_feriados_solicitados
         dict_temp.update(dict_feriado)
         self.dict_feriados_solicitados = dict_temp
         return data
 
+    def remove(self, nome):
+        """
+        Excluí feriado do objeto "Feraidos".
+        Ideal quando se utiliza a função "add_all", para adicionar todos,
+        sendo possível remover um ou outro feriado.
+
+        :param nome: Nome do feriado
+        :type nome: string
+        :raises Warning: Nome do feriado precisa ser um item dos
+        "feriados_disponiveis".
+        :return: Data do feriado removido do objeto "Feriados"
+        :rtype: date
+        """
+        if nome not in self.feriados_disponiveis:
+            fer = '\n'.join(self.feriados_disponiveis)
+            raise Warning(
+                f'O feriado precisa ser um dos listados abaixo\n{fer}'
+            )
+        # Feriados Solicitados
+        dict_temp = self.dict_feriados_solicitados
+        feriado_del = dict_temp.pop(nome)
+        self.dict_feriados_solicitados = dict_temp
+        return feriado_del['data']
+
+    def create_table(self):
+        """
+        Cria uma tabela de Feriados, em formato "pandas",
+        contendo os feriados adicionados individualmente,
+        ou total (com o método "add_all()").
+
+        Apresenta diversas descrições e atributos que
+        podem ser customizadas caso o usuário optei por
+        adicionar os feriados individualmente.
+
+        :return: Tabela com Feriados
+        :rtype: dataframe
+        """
+        # Adjust Table
+        if len(self.dict_feriados_solicitados) == 0:
+            raise Warning('Necessário Adicionar feriados!')
+
+        dataframe = pd.DataFrame.from_dict(
+            self.dict_feriados_solicitados, orient='index'
+        )
+        # df = df[pd.notna(df['data'])]
+        df = dataframe.sort_values(['data'], ascending=True)
+        df['data'] = pd.to_datetime(df['data'])
+        df['dia_semama'] = df['data'].dt.day_name(locale='PT')
+        df = df.reset_index(drop=True)
+        df = df.rename({'nome_alternativo': 'nome'}, axis=1)
+        df = df[['data', 'dia_semama', 'nome', 'feriado', 'tipo', 'obs']]
+        return df
+
+    def create_list(self, tipo='datetime'):
+        """
+        Cria uma lista de Feriados, em formato "date" ou "datetime",
+        contendo os feriados adicionados individualmente,
+        ou total (com o método "add_all").
+
+        Ideal para utilizar com a biblioteca "dateutil".
+
+        :param tipo: Tipo de lista, defaults to "datetime"
+        :type tipo: str, optional
+        :raises Warning: Lista precisa ser "date" ou "datetime"
+        :return: Lista dos Feriados
+        :rtype: list
+        """
+
+        if tipo not in ['date', 'datetime']:
+            raise Warning(
+                'É necessário que o formato seja "date" ou "datetime"!'
+            )
+
+        # Cria Tabela
+        df = self.create_table()
+
+        # sss
+        if tipo == 'date':
+            return [datetime.date(x) for x in df['data']]
+
+        elif tipo == 'datetime':
+            return [
+                datetime(
+                    year=x.year,
+                    month=x.month,
+                    day=x.day,
+                    hour=0,
+                    minute=0,
+                    second=0,
+                )
+                for x in df['data']
+            ]
+
     def next_feriado(self):
         """
-        _summary_
+        Define quando é o próximo feriado,
+        a partir do dia de hoje!
 
-        :return: _description_
-        :rtype: _type_
+        :return: Dia do próximo feriado
+        :rtype: date
         """
         # Pega dia de hoje
-        pivot = date.today()
-        items = self.create_list()
+        data = date.today()
+        items = self.create_list(tipo='date')
 
         # Lista de Datas
         list_res = []
         for x in items:
-            list_res.append((x - pivot).days)
+            list_res.append((x - data).days)
 
         # ddd
         n_days_holiday = min(n for n in list_res if n > 0)
-        return pivot + timedelta(days=n_days_holiday)
+        return data + timedelta(days=n_days_holiday)
 
     def __repr__(self):
         if len(self.dict_feriados_solicitados) == 0:
             return 'Não foram adicionados feriados'
 
         else:
             df = self.create_table()
@@ -401,15 +439,14 @@
     """
     Classe para manejar mais de um conjunto de feriados
     Idealizado para trabalhar com feriados de vários anos distintos
     """
 
     def __init__(self):
         self.tabelas_feriados = None
-        # self.df = None
         pass
 
     def create_table(self, tabelas_feriados):
         """
         _summary_
 
         :param tabelas_feriados: _description_
@@ -437,30 +474,52 @@
 
         df = pd.concat(objs=list_dfs, ignore_index=True)
         df = df.sort_values(['data'], ascending=True)
         df = df.reset_index(drop=True)
         # self.df = df
         return df
 
-    def create_list(self):
+    def create_list(self, tipo='datetime'):
         """
         Cria uma lista de Feriados, em formato datetime,
         contendo os feriados adicionados individualmente,
         ou total (com o método "all()")
 
+        :param tipo: Tipo de lista, defaults to 'datetime'
+        :type tipo: str, optional
+        :raises Warning: Lista precisa ser 'date' ou 'datetime'
         :return: Lista dos Feriados
         :rtype: list
         """
+        if tipo not in ['date', 'datetime']:
+            raise Warning(
+                'É necessário que o formato seja "date" ou "datetime"!'
+            )
+
         # Cria Tabela
         df = self.create_table(self.tabelas_feriados)
-        list_feriados = list(df['data'])
+
+        # Tipos
+        if tipo == 'date':
+            list_feriados = [datetime.date(x) for x in df['data']]
+
+        elif tipo == 'datetime':
+            list_feriados = [
+                datetime(
+                    year=x.year,
+                    month=x.month,
+                    day=x.day,
+                    hour=0,
+                    minute=0,
+                    second=0,
+                )
+                for x in df['data']
+            ]
 
         # Results
-        list_feriados = [x for x in list_feriados if pd.notna(x)]
-        list_feriados = [datetime.date(x) for x in df['data']]
         print(f'Existe(m) {len(list_feriados)} feriado(s)')
         return list_feriados
 
     def __repr__(self):
         df = self.create_table(self.tabelas_feriados)
         # TODO: Adicionar o ano!
         feriados = '\n'.join(list(df['nome']))
@@ -469,18 +528,18 @@
 
 if __name__ == '__main__':
     # Resultados
     feriados = Feriados(ano=2023)
     feriados.add(nome='Natal')
     feriados.add_all()
 
-    # # Lista Todos
-    # feriados = Feriados(ano=2023)
-    # feriados.add_all()
+    # Lista Todos
+    feriados = Feriados(ano=2023)
+    feriados.add_all()
 
     # # Lista
-    lista_feriados = feriados.create_list()
+    lista_feriados = feriados.create_list(tipo='datetime')
     print(lista_feriados)
 
     # # Tabela
     df = feriados.create_table()
     print(df)
```

### Comparing `feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/PKG-INFO` & `feriados_brasileiros-0.0.3/feriados_brasileiros.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feriados-brasileiros
-Version: 0.0.2
+Version: 0.0.3
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,dados espaciais,geoprocessamento
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,75 +43,100 @@
 
 ---
 
 ## Como Usar?!
 
 A maneira mais simples é obter todos os feriados para um determinado ano. Dessa forma os atributos serão definidos por padrão.
 
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados
+```
+
+<br>
+
+---
+
+## Detalhes
+
+É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos para cada um dos feriados.
+
 Dentre os atributos existentes estão:
 
-- `nome`: Nome do Feriado;
-- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente;
+- `nome_alternativo`: Nome do Feriado;
+- `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
-from feriados_brasileiros import Feriados
+from feriados_brasileiros import datas
 
-# Lista Todos dos Feriados de um determinado Ano
+# Adiciona apenas um feriado de um determinado ano
 feriados = Feriados(ano=2023)
+feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
+feriados
+```
+
+<br>
+
+---
+
+## Remoção
+
+É possível remover feriados específicos, após ter adicionado todos!.
+
+```python
+from feriados_brasileiros import datas
+
+# Adiciona todos os feriados de um determinado ano
+feriados = datas.Feriados(ano=2023)
 feriados.add_all()
+feriados.remove('Domingo de Ramos')
+feriados.remove('Endoenças')
+feriados
 ```
 
 <br>
 
 ---
 
-## Detalhes
+## _Custom_
 
-É possível usar a ferramenta de uma maneira mais customizada, onde é possível ajustar todos os atributos (`nome`, `feriado`, `obs`) para cada um dos feriados.
+Também é possível adicioanr um feriado customizado.
 
 ```python
-# Lista Todos dos Feriados de um determinado Ano
-feriados = Feriados(ano=2023)
+from feriados_brasileiros import datas
 
-# Feriados Móveis
-feriados.add_carnaval_seg(nome='Segundona de Carnaval!')
-feriados.add_carnaval_ter()
-feriados.add_carnaval_qua(obs='Entrada no serviço após as 14h!')
-feriados.add_endoencas(obs='Endoenças: é feriado isso?!', feriado=False)
-feriados.add_paixao_cristo(nome='Sexta-feira Santa', obs='Paixão de Cristo')
-feriados.add_pascoa(obs='Quero chocolate!!')
-feriados.add_corpus_christ()
-
-# Feriados Fixos
-feriados.add_confraternizacao()
-feriados.add_aniversario_sao_paulo(feriado=False)
-feriados.add_tiradentes()
-feriados.add_trabalho()
-feriados.add_independencia(obs='Independência ou Morte!')
-feriados.add_padroeira()
-feriados.add_finados()
-feriados.add_proclamacao_republica(obs='Dia de ler sobre o arretado Ruy Barbosa!')
-feriados.add_consciencia_negra()
-feriados.add_vespera_natal(feriado=False)
-feriados.add_natal()
-feriados.add_reveillon(feriado=False)
+# Adiciona todos os feriados de um determinado ano, além de outras feriados customizados (municipais e estaduais, por exemplo)
+feriados = datas.Feriados(ano=2023)
+feriados.add_all()
+feriados.add_custom(
+    nome='Dia do Servidor Público',
+    mes=10,
+    dia=28,
+    feriado=True,
+    tipo='Fixo',
+)
+feriados
 ```
 
 <br>
 
 ---
 
 ## Resultados
 
 Seja qual for a opção escolhida para usar o programa, os resultados podem ser obtidos de duas formas distintas.
 
 ```python
 # Resultado em Lista
-lista_feriados = feriados.create_list()
+lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
 df = feriados.create_table()
 print(df.head())
 ```
 
@@ -127,11 +152,11 @@
 
 <br>
 
 ---
 
 ## _TODO_
 
-1. Ajustar documentação
+1. ~~Ajustar documentação~~
 2. ~~Incluir o dia da semana!~~
 3. ~~Implantar classe Calendário para pegar feriados de anos diversos~~
 4. ~~Add domingo de ramos~~
```

### Comparing `feriados_brasileiros-0.0.2/setup.py` & `feriados_brasileiros-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
-VERSION = (0, 0, 2)
+VERSION = (0, 0, 3)
 __version__ = '.'.join(map(str, VERSION))
 
 setup(
     name='feriados_brasileiros',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
```

