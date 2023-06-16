# Comparing `tmp/modelolinguagem-1.0.4.tar.gz` & `tmp/modelolinguagem-1.0.6.tar.gz`

## Comparing `modelolinguagem-1.0.4.tar` & `modelolinguagem-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/__init__.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelolinguagem.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/medidas.py
--rw-r--r--   0        0        0    36654 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/mensurador.py
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/__init__.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/modeloarguments.py
--rw-r--r--   0        0        0    26985 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/modelo/transformer.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/nlp/__init__.py
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/nlp/nlpmodulo.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilambiente.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilconstantes.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utilmodulo.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/modelolinguagem/util/utiltempo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/LICENSE
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/README.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 modelolinguagem-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/__init__.py
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/mcl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/mensurador/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/mensurador/medidas.py
+-rw-r--r--   0        0        0    36769 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/mensurador/mensurador.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/modelo/__init__.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/modelo/modeloarguments.py
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/pln/__init__.py
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/utilambiente.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/utilconstantes.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/utiltempo.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/modelolinguagem/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/LICENSE
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 modelolinguagem-1.0.6/PKG-INFO
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/modelolinguagem.py` & `modelolinguagem-1.0.6/modelolinguagem/mcl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Import das bibliotecas.
 import logging  # Biblioteca de logging
 
 # Biblioteca dos modelos de linguagem
-from .modelo.modeloarguments import ModeloArgumentos
-from .nlp.nlpmodulo import *
-from .util.utilconstantes import *
-from .mensurador.mensuradorenum import *
-from .mensurador.mensurador import Mensurador
-from .modelo.transformer import *
+from modelolinguagem.modelo.modeloarguments import ModeloArgumentos
+from modelolinguagem.pln.pln import PLN
+from modelolinguagem.util.utilconstantes import *
+from modelolinguagem.mensurador.mensuradorenum import *
+from modelolinguagem.mensurador.mensurador import Mensurador
+from modelolinguagem.modelo.transformer import Transformer
 
 logger = logging.getLogger(__name__)
 
 # Definição dos parâmetros do Modelo para os cálculos das Medidas
 modelo_argumentos = ModeloArgumentos(
         max_seq_len=512,
         pretrained_model_name_or_path="neuralmind/bert-base-portuguese-cased", # Nome do modelo de linguagem pré-treinado Transformer
-        modelo_spacy="pt_core_news_lg", # Nome do modelo de linguagem da ferramenta de NLP
+        modelo_spacy="pt_core_news_lg", # Nome do modelo de linguagem da ferramenta de PLN
         do_lower_case=False,            # default True
         output_attentions=False,        # default False
         output_hidden_states=True,      # default False  /Retornar os embeddings das camadas ocultas  
         camadas_embeddings = 2,         # 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últiamas/5-Todas
         estrategia_pooling=0,           # 0 - MEAN estratégia média / 1 - MAX  estratégia maior
         palavra_relevante=0             # 0 - Considera todas as palavras das sentenças / 1 - Desconsidera as stopwords / 2 - Considera somente as palavras substantivas
         )
@@ -27,27 +27,27 @@
 class ModeloLinguagem:
     
     ''' 
     Carrega e cria um modelo de Linguagem, que pode ser usado para gerar embeddings de tokens, palavras, sentenças e textos.
      
     Parâmetros:
     `pretrained_model_name_or_path` - Se for um caminho de arquivo no disco, carrega o modelo a partir desse caminho. Se não for um caminho, ele primeiro faz o download do repositório de modelos do Huggingface com esse nome. Valor default: 'neuralmind/bert-base-portuguese-cased'.                  
-    `modelo_spacy` - Nome do modelo a ser instalado e carregado pela ferramenta de nlp spaCy. Valor default 'pt_core_news_lg'.                       
+    `modelo_spacy` - Nome do modelo a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.                       
     `camadas_embeddings` - Especifica de qual camada ou camadas será recuperado os embeddings do transformer. Valor defaul '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últiamas/5-Todas.       
     ''' 
     
     # Construtor da classe
     def __init__(self, pretrained_model_name_or_path="neuralmind/bert-base-portuguese-cased", 
                        modelo_spacy="pt_core_news_lg",
                        camadas_embeddings=2):
                        
         # Parâmetro recebido para o modelo de linguagem
         modelo_argumentos.pretrained_model_name_or_path = pretrained_model_name_or_path
                
-        # Parâmetro recebido para o modelo da ferramenta de nlp
+        # Parâmetro recebido para o modelo da ferramenta de pln
         modelo_argumentos.modelo_spacy = modelo_spacy
                 
         # Carrega o modelo de linguagem da classe transformador
         self.transformer_model = Transformer(modelo_args=modelo_argumentos)
     
         # Recupera o modelo.
         self.model = self.transformer_model.get_auto_model()
@@ -58,20 +58,20 @@
         # Especifica de qual camada utilizar os embeddings        
         logger.info("Utilizando embeddings do modelo da {} camada(s).".format(listaTipoCamadas[modelo_argumentos.camadas_embeddings][3]))
                     
         # Especifica camadas para recuperar os embeddings
         modelo_argumentos.camadas_embeddings = camadas_embeddings
       
         # Carrega o spaCy
-        self.nlp = NLP(modelo_args=modelo_argumentos)
+        self.pln = PLN(modelo_args=modelo_argumentos)
                         
         # Constroi um mensurador
         self.mensurador = Mensurador(modelo_args=modelo_argumentos, 
                                      transformer_model=self.transformer_model, 
-                                     nlp=self.nlp)        
+                                     pln=self.pln)        
     
         logger.info("Classe ModeloLinguagem carregada: {}.".format(modelo_argumentos))
     
     def defineEstrategiaPooling(self, estrategiaPooling):
         ''' 
         Define a estratégia de pooling para os parâmetros do modelo.
 
@@ -213,11 +213,10 @@
 
     def get_transformer_model(self):
         return self.transformer_model
         
     def get_mensurador(self):
         return self.mensurador        
         
-    def get_nlp(self):
-        return self.nlp          
-        
-        
+    def get_pln(self):
+        return self.pln          
+
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/mensurador/medidas.py` & `modelolinguagem-1.0.6/modelolinguagem/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/mensurador/mensurador.py` & `modelolinguagem-1.0.6/modelolinguagem/mensurador/mensurador.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # Import das bibliotecas.
 import logging  # Biblioteca de logging
 import torch # Biblioteca de aprendizado de máquina
 
 # Import de bibliotecas próprias
-from ..util.utilmodulo import *
-from ..util.utiltempo import *
-from ..util.utilarquivo import *
-from ..util.utilconstantes import *
-
-from ..nlp.nlpmodulo import *
-from .medidas import *
-from .mensuradorenum import *
+from modelolinguagem.util.utiltexto import *
+from modelolinguagem.util.utiltempo import *
+from modelolinguagem.util.utilarquivo import *
+from modelolinguagem.util.utilconstantes import *
+
+from modelolinguagem.pln.pln import *
+from modelolinguagem.mensurador.medidas import *
+from modelolinguagem.mensurador.mensuradorenum import *
 
 logger = logging.getLogger(__name__)
 
 class Mensurador:
 
     ''' 
     Realiza mensurações em textos.
      
     Parâmetros:
     `modelo_args` - Parâmetros do modelo de linguagem.
     `transformer_model` - Modelo de linguagem carregado.
-    `nlp` - Processador de linguagem natural.
+    `pln` - Processador de linguagem natural.
     ''' 
 
     # Construtor da classe
-    def __init__(self, modelo_args, transformer_model, nlp):
+    def __init__(self, modelo_args, transformer_model, pln):
     
         # Parâmetros do modelo
         self.model_args = modelo_args
     
         # Recupera o objeto do transformer.
         self.transformer_model = transformer_model
     
         # Recupera o modelo.
         self.model = transformer_model.get_auto_model()
     
         # Recupera o tokenizador.     
         self.tokenizer = transformer_model.get_tokenizer()
         
-        # Recupera a classe NLP
-        self.nlp = nlp
+        # Recupera a classe PLN
+        self.pln = pln
         
         logger.info("Classe Mensurador carregada: {}.".format(modelo_args))
       
     # ============================
     def getEmbeddingsTodasCamadas(self, texto):    
         '''   
         Retorna os embeddings de todas as camadas de um texto.
@@ -514,15 +514,15 @@
         '''
           
         # Tokeniza o texto
         textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Remove as stopword da sentença
-        sentencaSemStopWord = self.nlp.removeStopWord(sentenca)
+        sentencaSemStopWord = self.pln.removeStopWord(sentenca)
 
         # Tokeniza a sentença sem stopword
         sentencaTokenizadaSemStopWord =  self.transformer_model.getTextoTokenizado(sentencaSemStopWord)
         #print(sentencaTokenizadaSemStopWord)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizadaSemStopWord.remove('[CLS]')
@@ -576,15 +576,15 @@
         '''
 
         # Tokeniza o texto
         textoTokenizado =  self.transformer_model.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Retorna as palavras relevantes da sentença do tipo especificado
-        sentencaSomenteRelevante = self.nlp.retornaPalavraRelevante(sentenca, self.model_args.palavra_relevante)
+        sentencaSomenteRelevante = self.pln.retornaPalavraRelevante(sentenca, self.model_args.palavra_relevante)
 
         # Tokeniza a sentença 
         sentencaTokenizadaSomenteRelevante =  self.transformer_model.getTextoTokenizado(sentencaSomenteRelevante)
 
         # Remove os tokens de início e fim da sentença
         sentencaTokenizadaSomenteRelevante.remove('[CLS]')
         sentencaTokenizadaSomenteRelevante.remove('[SEP]')
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/mensurador/mensuradorenum.py` & `modelolinguagem-1.0.6/modelolinguagem/mensurador/mensuradorenum.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/modelo/modeloarguments.py` & `modelolinguagem-1.0.6/modelolinguagem/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/modelo/transformer.py` & `modelolinguagem-1.0.6/modelolinguagem/modelo/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 # Biblioteca de tipos
 from typing import List, Dict, Optional, Union, Tuple
 # Biblioteca de manipulação sistema
 import os
 
 # Biblioteca dos modelos de linguagem
-from .modeloarguments import ModeloArgumentos
+from modelolinguagem.modelo.modeloarguments import ModeloArgumentos
 
 logger = logging.getLogger(__name__)
 
 class Transformer(nn.Module):
     '''
     Huggingface AutoModel para gerar embeddings de token, palavra, sentença ou texto.
     Carrega a classe correta, por exemplo BERT / RoBERTa etc.
@@ -310,30 +310,30 @@
             return -1
 
 
     def getTokensEmbeddingsPOSSentenca(self, 
                                        embedding_documento, 
                                        token_MCL_documento,                                       
                                        sentenca,
-                                       NLP):
+                                       pln):
         '''    
           Retorna os tokens, as postagging e os embeddings dos tokens igualando a quantidade de tokens do spaCy com a tokenização do MCL de acordo com a estratégia. 
           Utiliza duas estratégias para realizar o pooling de tokens que forma uma palavra.
             - Estratégia MEAN para calcular a média dos embeddings dos tokens que formam uma palavra.
             - Estratégia MAX para calcular o valor máximo dos embeddings dos tokens que formam uma palavra.
         '''
        
         #Guarda os tokens e embeddings
         lista_tokens = []
         lista_tokens_OOV = []
         lista_embeddings_MEAN = []
         lista_embeddings_MAX = []
         
         # Gera a tokenização e POS-Tagging da sentença    
-        sentenca_token, sentenca_pos = NLP.getListaTokensPOSSentenca(sentenca)
+        sentenca_token, sentenca_pos = pln.getListaTokensPOSSentenca(sentenca)
 
         # print("\nsentenca          :",sentenca)    
         # print("sentenca_token      :",sentenca_token)
         # print("len(sentenca_token) :",len(sentenca_token))    
         # print("sentenca_pos        :",sentenca_pos)
         # print("len(sentenca_pos)   :",len(sentenca_pos))
         
@@ -497,24 +497,22 @@
             logger.info("lista_tokens               :{}.".format(lista_tokens))
             logger.info("len(lista_tokens)          :{}.".format(len(lista_tokens)))
             logger.info("sentenca_token             :{}.".format(sentenca_token))            
             logger.info("lista_embeddings_MEAN      :{}.".format(lista_embeddings_MEAN))
             logger.info("len(lista_embeddings_MEAN) :{}.".format(len(lista_embeddings_MEAN)))
             logger.info("lista_embeddings_MAX       :{}.".format(lista_embeddings_MAX))
             logger.info("len(lista_embeddings_MAX)  :{}.".format(len(lista_embeddings_MAX)))
-            
        
         del embedding_sentenca
         del token_MCL_documento
         del sentenca_tokenizada_MCL
         del sentenca_token
 
         return lista_tokens, sentenca_pos, lista_tokens_OOV, lista_embeddings_MEAN, lista_embeddings_MAX
 
-
     # ============================   
     def get_dimensao_embedding(self) -> int:
         '''
         Retorna a dimensão do embedding
         '''
         return self.auto_model.config.hidden_size
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/nlp/nlpmodulo.py` & `modelolinguagem-1.0.6/modelolinguagem/pln/pln.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,56 +2,56 @@
 import logging  # Biblioteca de logging
 import os # Biblioteca de manipulação de arquivos
 import spacy # Biblioteca do spaCy
 from spacy.util import filter_spans
 from spacy.matcher import Matcher
 
 # Import de bibliotecas próprias
-from ..util.utilmodulo import *
-from ..util.utiltempo import *
-from ..util.utilarquivo import *
-from ..util.utilambiente import *
-from ..mensurador.mensuradorenum import *
+from modelolinguagem.util.utiltexto import *
+from modelolinguagem.util.utiltempo import *
+from modelolinguagem.util.utilarquivo import *
+from modelolinguagem.util.utilambiente import *
+from modelolinguagem.mensurador.mensuradorenum import *
 
 logger = logging.getLogger(__name__)
 
-class NLP():
+class PLN():
 
     ''' 
     Realiza o processamento de linguagem natural.
      
     Parâmetros:
-    `nome_pln` - Nome da ferramenta de PLN a ser carregada.    
+    `modelo_args` - Parâmetros da classe PLN a ser carregado.    
     ''' 
 
     # Construtor da classe
     def __init__(self, modelo_args):
     
         # Parâmetros do modelo
         self.modelo_args = modelo_args
         
         #Instala o spaCy
         InstaladorModelo(modelo_args=modelo_args)
         
         #Carrega o modelo do spacy
         self.carrega()
             
-        logger.info("Classe NLP carregada: {}.".format(modelo_args))    
+        logger.info("Classe PLN carregada: {}.".format(modelo_args))    
             
     # ============================    
     def carrega(self):
         '''
-        Realiza o carregamento da ferramenta de NLP.
+        Realiza o carregamento da ferramenta de PLN.
      
         '''
        
         # Carrega o modelo spacy            
-        self.model_nlp = spacy.load(self.modelo_args.modelo_spacy)    
+        self.model_pln = spacy.load(self.modelo_args.modelo_spacy)    
         # Opção para remover funcionalidades
-        #self.model_nlp = spacy.load(self.modelo_args.modelo_spacy,disable=['tokenizer', 'lemmatizer', 'ner', 'parser', 'textcat', 'custom'])                
+        #self.model_pln = spacy.load(self.modelo_args.modelo_spacy,disable=['tokenizer', 'lemmatizer', 'ner', 'parser', 'textcat', 'custom'])                
         logger.info("Modelo spaCy versão {} carregado!".format(self.modelo_args.modelo_spacy))    
     
     # ============================
     
     def getPOSTaggingUniversalTraduzido(postagging):
         '''
         Retorna a tradução das POS-Tagging.
@@ -89,19 +89,19 @@
         else:
             traduzido = "NA" 
         return traduzido
     
     # ============================
     def getStopwords(self):
         '''
-        Recupera as stop words do model_nlp(Spacy).
+        Recupera as stop words do model_pln(Spacy).
                 
         '''
         
-        spacy_stopwords = self.model_nlp.Defaults.stop_words
+        spacy_stopwords = self.model_pln.Defaults.stop_words
         
         return spacy_stopwords 
 
     # ============================
     def removeStopWord(self, texto):
         '''
         Remove as stopwords de um texto.
@@ -132,15 +132,15 @@
         `tipo_palavra_relevante` - Tipo de palavra relevante a ser selecionada.
         
         Retorno:
         `textoComRelevantesConcatenado` - Texto somente com as palavras relevantes.
         '''
       
         # Realiza o parsing no texto usando spacy
-        doc = self.model_nlp(texto)
+        doc = self.model_pln(texto)
 
         # Retorna a lista das palavras relevantes de um tipo
         textoComRelevantes = [token.text for token in doc if token.pos_ == tipo_palavra_relevante]
 
         # Concatena o texto com as palavras relevantes
         textoComRelevantesConcatenado = ' '.join(textoComRelevantes)
 
@@ -154,15 +154,15 @@
         
         Parâmetros:
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
                  
         '''
 
         # Aplica sentenciação do spacy no texto
-        doc = self.model_nlp(texto) 
+        doc = self.model_pln(texto) 
 
         # Lista para as sentenças
         lista = []
         # Percorre as sentenças
         for sentenca in doc.sents: 
             # Adiciona as sentenças a lista
             lista.append(str(sentenca))
@@ -193,26 +193,26 @@
         gramaticav3 =  [
                         {"POS": "AUX", "OP": "?"},  #Verbos auxiliar 
                         {"POS": "AUX", "OP": "?", "DEP": {"IN": ["cop"]}},  #Verbos auxiliar de ligação (AUX+(cop))
                         {"POS": "ADJ", "OP": "+", "DEP": {"IN": ["ROOT"]}}, 
                         {"POS": "AUX", "OP": "?"}  #Verbos auxiliar 
                        ] 
 
-        matcherv = Matcher(nlp.vocab)
+        matcherv = Matcher(model_pln.vocab)
                  
         matcherv.add("frase verbal", [gramaticav1])
         matcherv.add("frase verbal", [gramaticav2])
         matcherv.add("frase verbal", [gramaticav3])
 
         #Processa o período        
         if isinstance(texto, str):            
-            doc1 = model_nlp(texto)
+            doc1 = model_pln(texto)
         else:
             #Processa o período
-            doc1 = model_nlp(texto.text)
+            doc1 = model_pln(texto.text)
           
         # Chama o mather para encontrar o padrão
         matches = matcherv(doc1)
 
         padrao = [doc1[start:end] for _, start, end in matches]
 
         #elimina as repetições e sobreposições
@@ -235,15 +235,15 @@
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
                  
         '''
         
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
-            doc = self.model_nlp(texto)
+            doc = self.model_pln(texto)
         else:
             doc = texto
 
         # Retorna inteiros que mapeiam para classes gramaticais
         conta_dicionarios = doc.count_by(spacy.attrs.IDS["POS"])
 
         # Dicionário com as tags e quantidades
@@ -263,15 +263,15 @@
         Parâmetros:
         `texto` - Um texto a ser convertido em uma lista de sentenças.           
                  
         '''
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
-            doc = self.model_nlp(texto)
+            doc = self.model_pln(texto)
         else:
             doc = texto
 
         # Retorna inteiros que mapeiam para classes gramaticais
         conta_dicionarios = doc.count_by(spacy.attrs.IDS["POS"])
 
         # Dicionário com as tags e quantidades    
@@ -314,15 +314,15 @@
         `texto` - Um texto a ser recuperado os tokens.
                  
         '''
 
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
-            doc = self.model_nlp(texto)
+            doc = self.model_pln(texto)
         else:
             doc = texto
 
         # Lista dos tokens
         lista = []
 
         # Percorre a sentença adicionando os tokens
@@ -340,15 +340,15 @@
         `texto` - Um texto a ser recuperado as POS-Tagging.
                  
         '''
 
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
-            doc = self.model_nlp(texto)
+            doc = self.model_pln(texto)
         else:
             doc = texto
 
         # Lista dos tokens
         lista = []
 
         # Percorre a sentença adicionando os tokens
@@ -365,15 +365,15 @@
         Parâmetros:
         `texto` - Um texto a ser recuperado as listas de tokens e POS-Tagging.
                  
         '''
         # Verifica se o texto não foi processado pelo spaCy  
         if type(texto) is not spacy.tokens.doc.Doc:
             # Realiza o parsing no spacy
-            doc = self.model_nlp(texto)
+            doc = self.model_pln(texto)
         else:
             doc = texto
 
         # Lista dos tokens
         lista_tokens = []
         lista_pos = []
 
@@ -406,16 +406,14 @@
             if token.lower() not in stopwords:
                 lista.append(token)
 
         # Retorna a lista de tokens sem as stopwords
         return lista
 
     # ============================   
-    def get_model_nlp(self):
+    def get_model_pln(self):
         '''
-        Recupera o modelo de NLP.
+        Recupera o modelo de PLN.
         '''
-        return self.model_nlp
+        return self.model_pln
         
-   
-          
-         
+
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/util/utilambiente.py` & `modelolinguagem-1.0.6/modelolinguagem/util/utilambiente.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/util/utilarquivo.py` & `modelolinguagem-1.0.6/modelolinguagem/util/utilarquivo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging  # Biblioteca de logging
 import requests # Biblioteca de download
 from tqdm.notebook import tqdm as tqdm_notebook # Biblioteca para barra de progresso
 import os # Biblioteca para manipular arquivos
 import sys
 
 # Import de bibliotecas próprias
-from .utilmodulo import *
-from .utiltempo import *
-from .utilconstantes import *
+from modelolinguagem.util.utiltexto import *
+from modelolinguagem.util.utiltempo import *
+from modelolinguagem.util.utilconstantes import *
 
 logger = logging.getLogger(__name__)
 
 # ============================  
 def verificaDiretorioModeloLinguagem():
     '''    
     Verifica se existe o diretório modelo_linguagem no diretório corrente.
```

### Comparing `modelolinguagem-1.0.4/modelolinguagem/util/utilconstantes.py` & `modelolinguagem-1.0.6/modelolinguagem/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/util/utilmodulo.py` & `modelolinguagem-1.0.6/modelolinguagem/util/utiltexto.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/modelolinguagem/util/utiltempo.py` & `modelolinguagem-1.0.6/modelolinguagem/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/LICENSE` & `modelolinguagem-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelolinguagem-1.0.4/pyproject.toml` & `modelolinguagem-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "modelolinguagem"
-version = "1.0.4"
+version = "1.0.6"
 description = "Framework Multilingual para processamento de textos utilizando modelos de linguagem"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
```

### Comparing `modelolinguagem-1.0.4/PKG-INFO` & `modelolinguagem-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelolinguagem
-Version: 1.0.4
+Version: 1.0.6
 Summary: Framework Multilingual para processamento de textos utilizando modelos de linguagem
 Project-URL: repository, https://github.com/osmarbraz/modelolinguagem/
 Author-email: Osmar de Oliveira Braz Junior <osmar.braz@udesc.br>
 License: MIT License
         
         Copyright (c) 2023 Osmar de Oliveira Braz Junior
```

