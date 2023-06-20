# Comparing `tmp/texto_transformer-0.0.0.tar.gz` & `tmp/texto_transformer-0.0.1.tar.gz`

## Comparing `texto_transformer-0.0.0.tar` & `texto_transformer-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/requirements.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/__init__.py
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/textotransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/mensurador/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/mensurador/medidas.py
--rw-r--r--   0        0        0    36871 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/mensurador/mensurador.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/modelo/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/modelo/modeloarguments.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/modelo/modeloenum.py
--rw-r--r--   0        0        0    28419 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/modelo/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/pln/__init__.py
--rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/pln/pln.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/utilambiente.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/utilconstantes.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/utiltempo.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/textotransformer/util/utiltexto.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 texto_transformer-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/requirements.txt
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/target/pylist.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/__init__.py
+-rw-r--r--   0        0        0    40424 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/textotransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/medidas.py
+-rw-r--r--   0        0        0    36781 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/mensurador.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/modeloarguments.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/modeloenum.py
+-rw-r--r--   0        0        0    32796 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/pln/__init__.py
+-rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilambiente.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilconstantes.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utiltempo.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/LICENSE
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/PKG-INFO
```

### Comparing `texto_transformer-0.0.0/textotransformer/mensurador/mensurador.py` & `texto_transformer-0.0.1/textotransformer/mensurador/mensurador.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 class Mensurador:
 
     ''' 
     Realiza mensurações em textos.
      
     Parâmetros:
     `modelo_args` - Parâmetros do modelo de linguagem.
-    `transformer_model` - Modelo de linguagem carregado.
+    `transformer` - Modelo de linguagem carregado.
     `pln` - Processador de linguagem natural.
     ''' 
 
     # Construtor da classe
-    def __init__(self, modelo_args, transformer_model, pln):
+    def __init__(self, modelo_args, transformer, pln):
     
         # Parâmetros do modelo
         self.model_args = modelo_args
     
         # Recupera o objeto do transformer.
-        self.transformer_model = transformer_model
+        self.transformer = transformer
     
         # Recupera o modelo.
-        self.model = transformer_model.get_auto_model()
+        self.model = transformer.get_auto_model()
     
         # Recupera o tokenizador.     
-        self.tokenizer = transformer_model.get_tokenizer()
+        self.tokenizer = transformer.get_tokenizer()
         
         # Recupera a classe PLN
         self.pln = pln
         
         logger.info("Classe Mensurador carregada: {}.".format(modelo_args))
       
     # ============================
@@ -59,15 +59,15 @@
         `input_ids` - Input ids do texto.
         `attention_mask` - Máscara de atenção do texto
         `token_type_ids` - Token types ids do texto.
         `outputs` - Embeddings do texto.
         '''
 
         # Texto tokenizado
-        textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)
+        textoTokenizado =  self.transformer.getTextoTokenizado(texto)
 
         #print('O texto (', texto, ') tem tamanho = ', len(textoTokenizado), ' = ', textoTokenizado)
 
         # Recupera a quantidade tokens do texto tokenizado.
         qtdeTokens = len(textoTokenizado)
 
         #tokeniza o texto e retorna os tensores.
@@ -479,19 +479,19 @@
                                               sentenca):
         '''
         Retorna os embeddings de uma sentença com todas as palavras(ALL) a partir dos embeddings do texto.
         
         '''
             
         # Tokeniza o texto
-        textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)
+        textoTokenizado =  self.transformer.getTextoTokenizado(texto)
         #print(textoTokenizado)
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer_model.getTextoTokenizado(sentenca)
+        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
         #print(sentencaTokenizada)
         # Remove os tokens de início e fim da sentença
         sentencaTokenizada.remove('[CLS]')
         sentencaTokenizada.remove('[SEP]')    
         #print(len(sentencaTokenizada))
 
         # Localiza os índices dos tokens da sentença no texto
@@ -511,31 +511,31 @@
                                                 texto, 
                                                 sentenca):
         '''
         Retorna os embeddings de uma sentença sem stopwords(CLEAN) a partir dos embeddings do texto.
         '''
           
         # Tokeniza o texto
-        textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)  
+        textoTokenizado =  self.transformer.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Remove as stopword da sentença
         sentencaSemStopWord = self.pln.removeStopWord(sentenca)
 
         # Tokeniza a sentença sem stopword
-        sentencaTokenizadaSemStopWord =  self.transformer_model.getTextoTokenizado(sentencaSemStopWord)
+        sentencaTokenizadaSemStopWord =  self.transformer.getTextoTokenizado(sentencaSemStopWord)
         #print(sentencaTokenizadaSemStopWord)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizadaSemStopWord.remove('[CLS]')
         sentencaTokenizadaSemStopWord.remove('[SEP]')    
         #print(len(sentencaTokenizadaSemStopWord))
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer_model.getTextoTokenizado(sentenca)
+        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizada.remove('[CLS]')
         sentencaTokenizada.remove('[SEP]')  
         #print(sentencaTokenizada)
         #print(len(sentencaTokenizada))
 
@@ -573,31 +573,31 @@
                                                texto, 
                                                sentenca):
         '''
         Retorna os embeddings de uma sentença somente com as palavras relevantes(NOUN) de um tipo a partir dos embeddings do texto.
         '''
 
         # Tokeniza o texto
-        textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)  
+        textoTokenizado =  self.transformer.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Retorna as palavras relevantes da sentença do tipo especificado
         sentencaSomenteRelevante = self.pln.retornaPalavraRelevante(sentenca, self.model_args.palavra_relevante)
 
         # Tokeniza a sentença 
-        sentencaTokenizadaSomenteRelevante =  self.transformer_model.getTextoTokenizado(sentencaSomenteRelevante)
+        sentencaTokenizadaSomenteRelevante =  self.transformer.getTextoTokenizado(sentencaSomenteRelevante)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizadaSomenteRelevante.remove('[CLS]')
         sentencaTokenizadaSomenteRelevante.remove('[SEP]')  
         #print(sentencaTokenizadaSomenteRelevante)
         #print(len(sentencaTokenizadaSomenteRelevante))
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer_model.getTextoTokenizado(sentenca)
+        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizada.remove('[CLS]')
         sentencaTokenizada.remove('[SEP]')  
         #print(sentencaTokenizada)
         #print(len(sentencaTokenizada))
```

### Comparing `texto_transformer-0.0.0/textotransformer/modelo/modeloarguments.py` & `texto_transformer-0.0.1/textotransformer/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/textotransformer/modelo/modeloenum.py` & `texto_transformer-0.0.1/textotransformer/modelo/modeloenum.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # Biblioteca de Enum
 from enum import Enum 
 
 logger = logging.getLogger(__name__)
 
 # ============================
 class EstrategiasPooling(Enum):
-    MEAN = 0 # Média
-    MAX = 1 # Máximo
+    MEAN = 0 # Média / Use a média em cada dimensão sobre todos os tokens.
+    MAX = 1 # Máximo / Use o máximo em cada dimensão sobre todos os tokens.
 
 # ============================
 # EmbeddingsCamadas
 # Define um enum com as camadas a serem analisadas nos teste.
 # Cada elemento do enum 'EmbeddingsCamadas' é chamado de camada sendo formado por:
 #  - camada.value[0] = Índice da camada
 #  - camada.value[1] = Um inteiro com o índice da camada a ser avaliada. Pode conter valores negativos.
```

### Comparing `texto_transformer-0.0.0/textotransformer/modelo/transformer.py` & `texto_transformer-0.0.1/textotransformer/modelo/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Import das bibliotecas.
 
 # Biblioteca de logging
 import logging  
 # Biblioteca de aprendizado de máquina
 from torch import nn 
 import torch 
+from torch import Tensor, device
 # Biblioteca do transformer
 from transformers import AutoModel, AutoTokenizer, AutoConfig, T5Config, MT5Config
 # Biblioteca de manipulação json
 import json
 # Biblioteca de tipos
 from typing import List, Dict, Optional, Union, Tuple
 # Biblioteca de manipulação sistema
@@ -215,14 +216,89 @@
         for tokens in saida['tokens_texto_mcl']:
             if len(tokens) >= 512:
                 logger.info("Utilizando embeddings do modelo de: {}.".format(listaTipoCamadas[self.modelo_args.camadas_embeddings]))   
                         
         return saida
     
     # ============================           
+    def forward(self, texto):
+        '''
+        De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto. 
+        O retorno é um dicionário com token_embeddings, input_ids, attention_mask, token_type_ids, 
+        tokens_texto_mcl, texto_original  e all_layer_embeddings.
+        
+        Retorna os embeddings de todas as camadas de um texto.
+    
+        Parâmetros:
+        `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
+    
+        Retorna um dicionário com:            
+            token_embeddings uma lista com os embeddings da última camada
+            input_ids uma lista com os textos indexados.            
+            attention_mask uma lista com os as máscaras de atenção
+            token_type_ids uma lista com os tipos dos tokens.            
+            tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
+            texto_original uma lista com os textos originais.
+            all_layer_embeddings uma lista com os embeddings de todas as camadas.
+        '''
+
+        # Se o texto não estiver tokenizado, tokeniza
+        if not isinstance(texto, dict):
+            texto = self.tokenize(texto)
+    
+        # Recupera o texto preparado pelo tokenizador para envio ao modelo
+        dic_texto_tokenizado = {'input_ids': texto['input_ids'],                                 
+                                'attention_mask': texto['attention_mask']}
+        
+        # Se token_type_ids estiver no texto preparado copia para dicionário
+        if 'token_type_ids' in texto:
+            dic_texto_tokenizado['token_type_ids'] = texto['token_type_ids']
+
+        # Roda o texto através do modelo, e coleta todos os estados ocultos produzidos.
+        outputs = self.auto_model(**dic_texto_tokenizado, 
+                                  return_dict=False)
+        
+        # A avaliação do modelo retorna um número de diferentes objetos com base em
+        # como é configurado na chamada do método `from_pretrained` anterior. Nesse caso,
+        # porque definimos `output_hidden_states = True`, o terceiro item será o
+        # estados ocultos(hidden_states) de todas as camadas. Veja a documentação para mais detalhes:
+        # https://huggingface.co/transformers/model_doc/bert.html#bertmodel
+
+        # Retorno de model quando ´output_hidden_states=True´ é setado:    
+        # outputs[0] = last_hidden_state, outputs[1] = pooler_output, outputs[2] = hidden_states
+        # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.        
+        # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
+        
+        last_hidden_state = outputs[0]
+
+        # Adiciona os embeddings da última camada e os dados do texto preparado na saída
+        saida = {}
+        saida.update({'token_embeddings': last_hidden_state,  # Embeddings da última camada
+                      'input_ids': texto['input_ids'],
+                      'attention_mask': texto['attention_mask'],
+                      'token_type_ids': texto['token_type_ids'],        
+                      'tokens_texto_mcl': texto['tokens_texto_mcl'],
+                      'texto_original': texto['texto_original']
+                      }
+                     )
+
+        # output_hidden_states == True existem embeddings nas camadas ocultas
+        if self.auto_model.config.output_hidden_states:
+            # 2 é o índice da saída com todos os embeddings em outputs
+            all_layer_idx = 2
+            if len(outputs) < 3: #Alguns modelos apenas geram last_hidden_states e all_hidden_states
+                all_layer_idx = 1
+
+            hidden_states = outputs[all_layer_idx]
+            # Adiciona os embeddings de todas as camadas na saída
+            saida.update({'all_layer_embeddings': hidden_states})
+
+        return saida
+
+    # ============================           
     def getEmbeddings(self, texto):
         '''
         De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto. 
         O retorno é um dicionário com token_embeddings, input_ids, attention_mask, token_type_ids, 
         tokens_texto_mcl, texto_original  e all_layer_embeddings.
         
         Retorna os embeddings de todas as camadas de um texto.
@@ -326,15 +402,15 @@
         else:
             return -1
 
     def getTokensEmbeddingsPOSTexto(self, 
                                    embeddings_texto, 
                                    tokens_texto_mcl,                                       
                                    tokens_texto_concatenado,
-                                   model_pln):
+                                   pln):
         '''
         De um texto preparado(tokenizado) ou não, retorna os embeddings das palavras do texto. 
         Retorna 5 listas, os tokens(palavras), as postagging, tokens OOV, e os embeddings dos tokens igualando a quantidade de tokens do spaCy com a tokenização do MCL de acordo com a estratégia. 
         Utiliza duas estratégias para realizar o pooling de tokens que forma uma palavra.
             - Estratégia MEAN para calcular a média dos embeddings dos tokens que formam uma palavra.
             - Estratégia MAX para calcular o valor máximo dos embeddings dos tokens que formam uma palavra.
             
@@ -352,15 +428,15 @@
         #Guarda os tokens e embeddings de retorno
         lista_tokens = []
         lista_tokens_OOV_mcl = []
         lista_embeddings_MEAN = []
         lista_embeddings_MAX = []
         
         # Gera a tokenização e POS-Tagging da sentença    
-        lista_tokens_texto_pln, lista_pos_texto_pln = model_pln.getListaTokensPOSTexto(tokens_texto_concatenado)
+        lista_tokens_texto_pln, lista_pos_texto_pln = pln.getListaTokensPOSTexto(tokens_texto_concatenado)
 
         # print("\tokens_texto_concatenado    :",tokens_texto_concatenado)    
         # print("lista_tokens_texto_pln       :",lista_tokens_texto_pln)
         # print("len(lista_tokens_texto_pln)  :",len(lista_tokens_texto_pln))    
         # print("lista_pos_texto_pln          :",lista_pos_texto_pln)
         # print("len(lista_pos_texto_pln)     :",len(lista_pos_texto_pln))
         
@@ -565,8 +641,16 @@
     # ============================   
     def get_tokenizer(self):
         '''
         Recupera o tokenizador.
         '''
         return self.tokenizer
 
-
+    # ============================   
+    def batch_to_device(self, lote, target_device: device):
+        '''
+        Envia lote pytorch batch para um dispositivo (CPU/GPU)
+        '''
+        for key in lote:
+            if isinstance(lote[key], Tensor):
+                lote[key] = lote[key].to(target_device)
+        return lote
```

### Comparing `texto_transformer-0.0.0/textotransformer/pln/pln.py` & `texto_transformer-0.0.1/textotransformer/pln/pln.py`

 * *Files 12% similar despite different names*

```diff
@@ -153,26 +153,56 @@
         Retorna uma lista com as sentenças de um texto. Utiliza o spacy para dividir o texto em sentenças.
         
         Parâmetros:
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
                  
         '''
 
-        # Aplica sentenciação do spacy no texto
-        doc = self.model_pln(texto) 
+        # Verifica se o texto não foi processado pelo spaCy  
+        if type(texto) is not spacy.tokens.doc.Doc:
+            # Realiza o parsing no spacy
+            doc = self.model_pln(texto)
+        else:
+            doc = texto
 
         # Lista para as sentenças
         lista = []
         # Percorre as sentenças
         for sentenca in doc.sents: 
             # Adiciona as sentenças a lista
             lista.append(str(sentenca))
 
         return lista       
+
+    # ============================
+    def getListaSentencasTokensTexto(self, texto):
+        '''
+        Retorna duas listas, uma com as sentenças de um texto e outra com a lista de lista de tokens de cada sentença.
         
+        Parâmetros:
+        `texto` - Um texto a ser processado em uma lista de sentenças e tokens.           
+
+        Retorno:
+        `lista_sentencas` - Lista com as sentenças do texto.
+        `lista_tokens` - Lista com os tokens de cada sentença do texto.
+                 
+        '''
+
+        # Retorna uma lista com as sentenlas do texto        
+        lista_sentencas = self.getListaSentencasTexto(texto)
+
+        # Lista para os tokens
+        lista_tokens = []
+        # Percorre as sentenças
+        for sentenca in lista_sentencas:
+            # Adiciona os tokens a lista
+            lista_tokens.append(self.getListaTokensSentenca(sentenca))
+
+        return lista_sentencas, lista_tokens
+
     # ============================
     def getVerbosTexto(self, texto):
         
         # (verbo normal como auxilar ou auxilar) + vários verbos auxiliares +verbo principal ou verbo auxiliar
         gramaticav1 =  [
                         {"POS": "AUX", "OP": "?", "DEP": {"IN": ["aux","aux:pass"]}},  #verbo auxiliar                                  
                         {"POS": "VERB", "OP": "?", "DEP": {"IN": ["ROOT","aux","xcomp","aux:pass"]}},  #verbo normal como auxiliar
```

### Comparing `texto_transformer-0.0.0/textotransformer/util/utilambiente.py` & `texto_transformer-0.0.1/textotransformer/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/textotransformer/util/utilarquivo.py` & `texto_transformer-0.0.1/textotransformer/util/utilarquivo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/textotransformer/util/utilconstantes.py` & `texto_transformer-0.0.1/textotransformer/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/textotransformer/util/utiltempo.py` & `texto_transformer-0.0.1/textotransformer/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/textotransformer/util/utiltexto.py` & `texto_transformer-0.0.1/textotransformer/util/utiltexto.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,44 +8,63 @@
 import unicodedata 
 from collections import Counter
 from functools import reduce
 
 logger = logging.getLogger(__name__)
 
 # ============================  
-def removeAcentos(texto):   
+def convertTextoUtf8(texto):   
     '''    
-    Remove acentos de um texto.
+    Converte um texto para utf-8.
     
     Parâmetros:
-   `texto` - Texto a ser removido os acentos.
+   `texto` - Texto a ser convertido para utf-8.
+
+    Retorno:
+    Texto convertido para utf-8.
     '''
     
     try:
-        text = unicode(texto, 'utf-8')
+        texto = texto.encode('utf-8')
     except (TypeError, NameError): 
         pass
+
+    return texto
+# ============================  
+def removeAcentos(texto):   
+    '''    
+    Remove acentos de um texto.
     
+    Parâmetros:
+   `texto` - Texto a ser removido os acentos.
+
+    Retorno:
+    Texto sem acentos.
+    '''
+    
+    texto = convertTextoUtf8(texto)    
     texto = unicodedata.normalize('NFD', texto)
     texto = texto.encode('ascii', 'ignore')
     texto = texto.decode("utf-8")
     
     return str(texto)
 
 # ============================  
 def limpaTexto(texto):    
     '''    
     Remove acentos e espaços e outros caracteres de um texto.
     
     Parâmetros:
    `texto` - Texto a ser limpo.
     '''
-    
+    # Converte para minúsculo
     texto = removeAcentos(texto.lower())
+    # Remove espaços em branco
     texto = re.sub('[ ]+', '_', texto)
+    # Remove caracteres especiais
     texto = re.sub('[^.0-9a-zA-Z_-]', '', texto)
     
     return texto
     
 # ============================  
 def remove_tags(texto):
     '''
@@ -55,15 +74,14 @@
     `texto` - Texto com tags a serem removidas.      
     '''
      
     textoLimpo = re.compile('<.*?>')
      
     return re.sub(textoLimpo, '', texto)
 
-
 # ============================
 def encontrarIndiceSubLista(lista, sublista):
     '''
     Localiza os índices de início e fim de uma sublista em uma lista.
     
     Parâmetros:
     `lista` - Uma lista.
@@ -114,8 +132,41 @@
     Parâmetros:
     `lista` - Uma lista contendo dicionários.           
     '''
     
     # Soma os dicionários da lista
     novodic = reduce(atualizaValor, (Counter(dict(x)) for x in lista))
  
-    return novodic        
+    return novodic
+
+def limpeza(texto):
+    '''
+    Realiza limpeza dos dados.
+        
+    Parâmetros:
+    `texto` - Um texto a ser limpo.      
+
+    Retorno:
+    `texto` - Texto limpo.  
+    '''
+    # Substitui \n por espaço em branco no documento
+    conta_caracter_barra_n = texto.count("\n")
+    if conta_caracter_barra_n > 0:
+        # Transforma \n em espaços em branco 
+        texto = texto.replace("\n"," ")
+
+    # Transforma em string e remove os espaços do início e do fim
+    texto = str(texto).strip()
+
+    # Conta texto com duas ou mais interrogação
+    conta_caracter_interrogacoes = texto.count("?")
+    if conta_caracter_interrogacoes > 1:
+        # Transforma 2 ou mais interrogações consecutivas em 1
+        texto = re.sub("\?+", "?", texto)
+        
+    # Conta caracteres em branco repetidos
+    conta_caracter_espacos = texto.count("  ")
+    if conta_caracter_espacos > 0:
+        # Transforma 2 ou mais caracteres em branco consecutivos em 1    
+        texto = re.sub("\W*\?+\W*", "? ", texto)
+        
+    return texto
```

### Comparing `texto_transformer-0.0.0/LICENSE` & `texto_transformer-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.0/README.md` & `texto_transformer-0.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 
 ## Instalação
 
 Para instalar o pacote, basta executar o comando abaixo:
 
 <pre><code>$ pip install texto-transformer</code></pre>
 
+## Uso
+
+Exemplo simples de uso do pacote:
+
+````python
+from textotransformer import TextoTransformer
+
+modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
+````
+
 ## Dependências
 - transformers==4.26.1
 - spacy==3.5.2
 
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

### Comparing `texto_transformer-0.0.0/pyproject.toml` & `texto_transformer-0.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "texto-transformer"
-version = "0.0.0"
+version = "0.0.1"
 description = "Texto Transformer: Framework multilingual para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
@@ -16,15 +16,16 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 keywords = ["Framework", "Transformer","embedding","texto", "sentença", "palavra", "token"]
 
 dependencies = ["transformers==4.26.1", 
-			    "spacy==3.5.2"]
+			    "spacy==3.5.2",
+                "tqdm==4.65.0"]
 
 [project.urls]
 repository = "https://github.com/osmarbraz/textotransformer/"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `texto_transformer-0.0.0/PKG-INFO` & `texto_transformer-0.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texto-transformer
-Version: 0.0.0
+Version: 0.0.1
 Summary: Texto Transformer: Framework multilingual para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer
 Project-URL: repository, https://github.com/osmarbraz/textotransformer/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
         
@@ -30,27 +30,38 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.0
 Requires-Dist: spacy==3.5.2
+Requires-Dist: tqdm==4.65.0
 Requires-Dist: transformers==4.26.1
 Description-Content-Type: text/markdown
 
 # Texto Transformer: Framework multilingual para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer
 
 Gera embeddings de textos, sentenças, palavras e tokens utilizando modelos contextualizados de linguagem multilingual baseados em Transformer.
 
 ## Instalação
 
 Para instalar o pacote, basta executar o comando abaixo:
 
 <pre><code>$ pip install texto-transformer</code></pre>
 
+## Uso
+
+Exemplo simples de uso do pacote:
+
+````python
+from textotransformer import TextoTransformer
+
+modelo = TextoTransformer("neuralmind/bert-base-portuguese-cased")
+````
+
 ## Dependências
 - transformers==4.26.1
 - spacy==3.5.2
 
 ## Licença
 
 Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
```

