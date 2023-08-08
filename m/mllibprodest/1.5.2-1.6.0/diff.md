# Comparing `tmp/mllibprodest-1.5.2.tar.gz` & `tmp/mllibprodest-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllibprodest-1.5.2.tar", last modified: Tue May 16 17:18:47 2023, max compression
+gzip compressed data, was "mllibprodest-1.6.0.tar", last modified: Tue Aug  8 20:40:48 2023, max compression
```

## Comparing `mllibprodest-1.5.2.tar` & `mllibprodest-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/
--rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/LICENSE
--rw-rw-r--   0 messias   (1000) messias   (1000)    25103 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)    24109 2023-05-16 17:03:16.000000 mllibprodest-1.5.2/README.md
--rw-rw-r--   0 messias   (1000) messias   (1000)     1024 2023-05-16 16:12:14.000000 mllibprodest-1.5.2/pyproject.toml
--rw-rw-r--   0 messias   (1000) messias   (1000)      190 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/setup.cfg
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     9117 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/interfaces.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     5308 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/provider.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/providers_types/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2037 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/local_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2303 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/minio_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     7927 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/mlflow_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     8476 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/shared_classes.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     6772 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/utils.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/validators/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/validators/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)    21483 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/validators/test.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest.egg-info/
--rw-rw-r--   0 messias   (1000) messias   (1000)    25103 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)      666 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/SOURCES.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)        1 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/dependency_links.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       65 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/requires.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       13 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/top_level.txt
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/
+-rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/LICENSE
+-rw-rw-r--   0 messias   (1000) messias   (1000)    25713 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)    24719 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/README.md
+-rw-rw-r--   0 messias   (1000) messias   (1000)     1023 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/pyproject.toml
+-rw-rw-r--   0 messias   (1000) messias   (1000)      190 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/setup.cfg
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.908053 mllibprodest-1.6.0/src/
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/src/mllibprodest/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/__init__.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/src/mllibprodest/initiators/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/initiators/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     5582 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/initiators/model_initiator.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     9876 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/interfaces.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     5308 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/provider.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/src/mllibprodest/providers_types/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/providers_types/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2037 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/providers_types/local_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2303 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/providers_types/minio_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     8019 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/providers_types/mlflow_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     8789 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/shared_classes.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    10452 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/utils.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/src/mllibprodest/validators/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/validators/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    21609 2023-08-08 20:38:59.000000 mllibprodest-1.6.0/src/mllibprodest/validators/test.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-08-08 20:40:48.912052 mllibprodest-1.6.0/src/mllibprodest.egg-info/
+-rw-rw-r--   0 messias   (1000) messias   (1000)    25713 2023-08-08 20:40:48.000000 mllibprodest-1.6.0/src/mllibprodest.egg-info/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)      753 2023-08-08 20:40:48.000000 mllibprodest-1.6.0/src/mllibprodest.egg-info/SOURCES.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)        1 2023-08-08 20:40:48.000000 mllibprodest-1.6.0/src/mllibprodest.egg-info/dependency_links.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       64 2023-08-08 20:40:48.000000 mllibprodest-1.6.0/src/mllibprodest.egg-info/requires.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       13 2023-08-08 20:40:48.000000 mllibprodest-1.6.0/src/mllibprodest.egg-info/top_level.txt
```

### Comparing `mllibprodest-1.5.2/LICENSE` & `mllibprodest-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.2/PKG-INFO` & `mllibprodest-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.5.2
+Version: 1.6.0
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
@@ -73,15 +73,15 @@
 # Obs.: Utilize as duas linhas abaixo, exatamente como apresentadas, para configurar o parâmetro 'Tracking URI' do MLflow 
 # nos seus códigos de testes. Dessa forma, quando subir para produção não haverá necessidade de modificá-las, pois lá
 # o parâmetro 'Tracking URI' será obtido diretamente através da variável de ambiente 'MLFLOW_TRACKING_URI'.
 if os.environ.get('MLFLOW_TRACKING_URI') is None:
     mlflow.set_tracking_uri('sqlite:///teste_mlflow.db')
 
 # Configura o experimento (se não existir, cria)
-mlflow.set_experiment(experiment_name="Teste sklearn")
+mlflow.set_experiment(experiment_name="Teste_sklearn")
 
 # Inicia uma execução do experimento (um experimento pode possuir várias execuções)
 mlflow.start_run(run_name="t1", description="teste 1")
 
 # Registra algumas informações adicionais no experimento (coloque as informações que julgar necessárias, no formato dict)
 tags = {"Projeto": "Teste", "team": "ML", "util": "Informação útil"}
 mlflow.set_tags(tags)
@@ -128,28 +128,28 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
+pip install mlflow==2.5.0 scikit-learn==1.3.0 matplotlib==3.7.2 numpy==1.25.2
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
 Abaixo segue uma listagem do conteúdo gerado pelo código de teste (obs.: essa parte do caminho vai ser diferente de 
-acordo com cada experimento/execução realizados: '1/f454220e01bd43e7b66c2354c20f0085'. O conteúdo da pasta também será 
+acordo com cada experimento/execução realizados: '1/9d01359d68034063867613196395388e'. O conteúdo da pasta também será 
 diferente de acordo com cada modelo).
 ```bash
-(env) user:~/testes/mlruns/1/f454220e01bd43e7b66c2354c20f0085/artifacts$ dir
-artefato.pkl  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
+(env) user:~/testes/mlruns/1/9d01359d68034063867613196395388e/artifacts$ dir
+artefato.pkl  estimator.html  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
 ```
 Dentro da pasta criada para testes também foi gerado um arquivo chamado '**teste_mlflow.db**', que é um pequeno banco 
 de dados [SQlite](https://www.sqlite.org), que serve para armazenar os modelos que foram registrados.
 
 - Inicie o servidor do MLflow;
 
 Perceba que a pasta '**mlruns**' e o arquivo '**teste_mlflow.db**' foram passados como parâmetros na hora de iniciar o 
@@ -159,16 +159,16 @@
 **DICA**: Abra um outro prompt de comando ou terminal diferente; entre na pasta onde se encontra o código para registro 
 dos experimentos/modelo; execute o comando para iniciar o servidor do MLflow de dentro desta pasta. Pois assim, você 
 conseguirá rodar o código e já observar os resultados sem ter que parar o servidor para liberar o prompt ou terminal.
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 
-- Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
-pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
+- Verifique se o experimento foi criado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
+pelo experimento/execução '**Teste_sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
 - Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
@@ -211,19 +211,18 @@
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
-Prodest. Porém, antes, é oporturno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
+Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
 componentes denominados *workers*, cuja codificação é de responsabilidade de quem está construindo o modelo. Na 
 ilustração abaixo é possível observar que os *workers* são acessados pelos componentes de apoio da *stack* para 
-permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo, desde que 
-sejam construídos *workers* dedicados para cada um deles.
+permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo.
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/stack-ml.png?raw=true)
 
 Existem dois tipos de *workers*:
 - **worker_pub**: Fornece os métodos necessários para publicação do modelo.
 - **worker_retrain**: Responsável pela avaliação do desempenho do modelo e retreinamento, se for preciso.
 
@@ -294,19 +293,19 @@
 *workers*. Dessa forma, à medida que você for produzindo o código e necessitar de instalar pacotes, esses serão 
 instalados nos ambientes virtuais criados. Quando terminar a implementação, basta você gerar os arquivos de 
 *requirements* com base no ambiente virtual de cada *worker* separadamente. Acredite, isso vai te ajudar bastante!
 
 Outro ponto importante antes de implementar as interfaces é saber que: para publicar o modelo será necessário a criação 
 de três artefatos obrigatórios, inclusive seguindo o mesmo nome (*case sensitive*). Estes artefatos devem ser 
 dicionários (dict) salvos com o [Pickle](https://docs.python.org/3/library/pickle.html) (utilize a função 
-'convert_artifact_to_pickle' quando estiver implementando as intefaces):
+'convert_artifact_to_pickle' quando estiver implementando as interfaces):
 
 - **TrainingParams.pkl**: Deve conter os parâmetros que você escolheu utilizar no treinamento do modelo. Não há 
-necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros 
-criados por você necessários para que o modelo funcione. Coloque o nome 
+necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros, 
+criados por você, necessários para que o modelo funcione. Coloque o nome 
 do parâmetro como nome da chave e o valor do parâmetro como valor da chave. Ex. baseado no *DecisionTreeClassifier*: 
 {'criterion': 'entropy', 'max_depth': '20', 'random_state': '77', 'meu_parametro_personalizado': 'teste'}. 
 
 
 - **TrainingDatasetsNames.pkl**: Deve conter os tipos de datasets e os nomes dos respectivos arquivos utilizados no
 treinamento do modelo. Exemplo: {'features': 'nome_arquivo_features', 'targets': 'nome_arquivo_targets'}.
 
@@ -329,36 +328,49 @@
 Para implementar as interfaces e construir os *workers* basta editar os *templates* conforme abaixo:
 
 **REGRAS**: Implemente todos os métodos solicitados respeitando os tipos dos parâmetros e de retorno. Não troque os 
 nomes dos parâmetros.
 
 **worker_pub**:
 
-- Abra o arquivo '**pub.py**', que se encontra na pasta '**worker_pub**', e implemente os métodos da interface 
+- Abra o arquivo '**pub1.py**', que se encontra na pasta '**worker_pub/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceCLF** através da classe **ModeloCLF**. Leia os comentários, eles te guiarão na implementação.
+ 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_pub**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
 
 **worker_retrain**:
 
-- Abra o arquivo '**retrain.py**', que se encontra na pasta '**worker_retrain**', e implemente os métodos da interface 
+- Abra o arquivo '**retrain1.py**', que se encontra na pasta '**worker_retrain/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceRETRAIN** através da classe **ModeloRETRAIN**. Leia os comentários, eles te guiarão na 
 implementação.
 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_retrain**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
+
+**NOTA**: É possível publicar um ou mais modelos utilizando uma mesma **Stack**. Para isso, basta fazer as devidas
+configurações de cada um dos modelos nos arquivos '**params.conf**' constantes nas pastas **worker_pub** e **worker_retrain**.
+
 A lib disponibiliza vários métodos úteis que auxiliarão na implementação das interfaces. 
 Todos os métodos estão documentados via [docstrings](https://peps.python.org/pep-0257/) que, geralmente, são 
 renderizadas pelas IDEs ou editores de código facilitando a leitura da documentação. Veja alguns métodos úteis disponíveis:
 
 - **make_log** - Criação do arquivo para geração de logs.
 - **load_datasets** - Carga de datasets.
 - **load_model** - Carga de modelos salvos.
 - **load_production_params**, **load_production_datasets_names**, **load_production_baseline** - Carga das informações 
 dos modelos publicados, salvas através dos artefatos obrigatórios.
 - **convert_artifact_to_pickle** - Conversão de um artefato para o formato pickle.
 - **convert_artifact_to_object** - Conversão de um artefato que está no formato pickle para o objeto de origem.
 
-Explore a documentação para saber das possibilidades de uso da lib.
+Explore a [documentação](https://prodest.github.io/mllibprodest) para saber das possibilidades de uso da lib.
 
 ### Teste o código produzido!
 O repositório da lib disponibiliza os scripts '**test_pub.py**' e '**test_retrain.py**' para realização de testes para 
 verificar se alguns requisitos solicitados estão sendo atendidos. Também é possível criar testes personalizados através da 
 implementação da função '**test**' que se encontra nos scripts '**mytest_pub.py**' e '**mytest_retrain.py**'. Todos 
 estes scripts estão nas pastas **worker_pub** e **worker_retrain**.
```

### Comparing `mllibprodest-1.5.2/README.md` & `mllibprodest-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 # Obs.: Utilize as duas linhas abaixo, exatamente como apresentadas, para configurar o parâmetro 'Tracking URI' do MLflow 
 # nos seus códigos de testes. Dessa forma, quando subir para produção não haverá necessidade de modificá-las, pois lá
 # o parâmetro 'Tracking URI' será obtido diretamente através da variável de ambiente 'MLFLOW_TRACKING_URI'.
 if os.environ.get('MLFLOW_TRACKING_URI') is None:
     mlflow.set_tracking_uri('sqlite:///teste_mlflow.db')
 
 # Configura o experimento (se não existir, cria)
-mlflow.set_experiment(experiment_name="Teste sklearn")
+mlflow.set_experiment(experiment_name="Teste_sklearn")
 
 # Inicia uma execução do experimento (um experimento pode possuir várias execuções)
 mlflow.start_run(run_name="t1", description="teste 1")
 
 # Registra algumas informações adicionais no experimento (coloque as informações que julgar necessárias, no formato dict)
 tags = {"Projeto": "Teste", "team": "ML", "util": "Informação útil"}
 mlflow.set_tags(tags)
@@ -107,28 +107,28 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
+pip install mlflow==2.5.0 scikit-learn==1.3.0 matplotlib==3.7.2 numpy==1.25.2
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
 Abaixo segue uma listagem do conteúdo gerado pelo código de teste (obs.: essa parte do caminho vai ser diferente de 
-acordo com cada experimento/execução realizados: '1/f454220e01bd43e7b66c2354c20f0085'. O conteúdo da pasta também será 
+acordo com cada experimento/execução realizados: '1/9d01359d68034063867613196395388e'. O conteúdo da pasta também será 
 diferente de acordo com cada modelo).
 ```bash
-(env) user:~/testes/mlruns/1/f454220e01bd43e7b66c2354c20f0085/artifacts$ dir
-artefato.pkl  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
+(env) user:~/testes/mlruns/1/9d01359d68034063867613196395388e/artifacts$ dir
+artefato.pkl  estimator.html  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
 ```
 Dentro da pasta criada para testes também foi gerado um arquivo chamado '**teste_mlflow.db**', que é um pequeno banco 
 de dados [SQlite](https://www.sqlite.org), que serve para armazenar os modelos que foram registrados.
 
 - Inicie o servidor do MLflow;
 
 Perceba que a pasta '**mlruns**' e o arquivo '**teste_mlflow.db**' foram passados como parâmetros na hora de iniciar o 
@@ -138,16 +138,16 @@
 **DICA**: Abra um outro prompt de comando ou terminal diferente; entre na pasta onde se encontra o código para registro 
 dos experimentos/modelo; execute o comando para iniciar o servidor do MLflow de dentro desta pasta. Pois assim, você 
 conseguirá rodar o código e já observar os resultados sem ter que parar o servidor para liberar o prompt ou terminal.
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 
-- Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
-pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
+- Verifique se o experimento foi criado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
+pelo experimento/execução '**Teste_sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
 - Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
@@ -190,19 +190,18 @@
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
-Prodest. Porém, antes, é oporturno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
+Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
 componentes denominados *workers*, cuja codificação é de responsabilidade de quem está construindo o modelo. Na 
 ilustração abaixo é possível observar que os *workers* são acessados pelos componentes de apoio da *stack* para 
-permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo, desde que 
-sejam construídos *workers* dedicados para cada um deles.
+permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo.
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/stack-ml.png?raw=true)
 
 Existem dois tipos de *workers*:
 - **worker_pub**: Fornece os métodos necessários para publicação do modelo.
 - **worker_retrain**: Responsável pela avaliação do desempenho do modelo e retreinamento, se for preciso.
 
@@ -273,19 +272,19 @@
 *workers*. Dessa forma, à medida que você for produzindo o código e necessitar de instalar pacotes, esses serão 
 instalados nos ambientes virtuais criados. Quando terminar a implementação, basta você gerar os arquivos de 
 *requirements* com base no ambiente virtual de cada *worker* separadamente. Acredite, isso vai te ajudar bastante!
 
 Outro ponto importante antes de implementar as interfaces é saber que: para publicar o modelo será necessário a criação 
 de três artefatos obrigatórios, inclusive seguindo o mesmo nome (*case sensitive*). Estes artefatos devem ser 
 dicionários (dict) salvos com o [Pickle](https://docs.python.org/3/library/pickle.html) (utilize a função 
-'convert_artifact_to_pickle' quando estiver implementando as intefaces):
+'convert_artifact_to_pickle' quando estiver implementando as interfaces):
 
 - **TrainingParams.pkl**: Deve conter os parâmetros que você escolheu utilizar no treinamento do modelo. Não há 
-necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros 
-criados por você necessários para que o modelo funcione. Coloque o nome 
+necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros, 
+criados por você, necessários para que o modelo funcione. Coloque o nome 
 do parâmetro como nome da chave e o valor do parâmetro como valor da chave. Ex. baseado no *DecisionTreeClassifier*: 
 {'criterion': 'entropy', 'max_depth': '20', 'random_state': '77', 'meu_parametro_personalizado': 'teste'}. 
 
 
 - **TrainingDatasetsNames.pkl**: Deve conter os tipos de datasets e os nomes dos respectivos arquivos utilizados no
 treinamento do modelo. Exemplo: {'features': 'nome_arquivo_features', 'targets': 'nome_arquivo_targets'}.
 
@@ -308,36 +307,49 @@
 Para implementar as interfaces e construir os *workers* basta editar os *templates* conforme abaixo:
 
 **REGRAS**: Implemente todos os métodos solicitados respeitando os tipos dos parâmetros e de retorno. Não troque os 
 nomes dos parâmetros.
 
 **worker_pub**:
 
-- Abra o arquivo '**pub.py**', que se encontra na pasta '**worker_pub**', e implemente os métodos da interface 
+- Abra o arquivo '**pub1.py**', que se encontra na pasta '**worker_pub/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceCLF** através da classe **ModeloCLF**. Leia os comentários, eles te guiarão na implementação.
+ 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_pub**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
 
 **worker_retrain**:
 
-- Abra o arquivo '**retrain.py**', que se encontra na pasta '**worker_retrain**', e implemente os métodos da interface 
+- Abra o arquivo '**retrain1.py**', que se encontra na pasta '**worker_retrain/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceRETRAIN** através da classe **ModeloRETRAIN**. Leia os comentários, eles te guiarão na 
 implementação.
 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_retrain**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
+
+**NOTA**: É possível publicar um ou mais modelos utilizando uma mesma **Stack**. Para isso, basta fazer as devidas
+configurações de cada um dos modelos nos arquivos '**params.conf**' constantes nas pastas **worker_pub** e **worker_retrain**.
+
 A lib disponibiliza vários métodos úteis que auxiliarão na implementação das interfaces. 
 Todos os métodos estão documentados via [docstrings](https://peps.python.org/pep-0257/) que, geralmente, são 
 renderizadas pelas IDEs ou editores de código facilitando a leitura da documentação. Veja alguns métodos úteis disponíveis:
 
 - **make_log** - Criação do arquivo para geração de logs.
 - **load_datasets** - Carga de datasets.
 - **load_model** - Carga de modelos salvos.
 - **load_production_params**, **load_production_datasets_names**, **load_production_baseline** - Carga das informações 
 dos modelos publicados, salvas através dos artefatos obrigatórios.
 - **convert_artifact_to_pickle** - Conversão de um artefato para o formato pickle.
 - **convert_artifact_to_object** - Conversão de um artefato que está no formato pickle para o objeto de origem.
 
-Explore a documentação para saber das possibilidades de uso da lib.
+Explore a [documentação](https://prodest.github.io/mllibprodest) para saber das possibilidades de uso da lib.
 
 ### Teste o código produzido!
 O repositório da lib disponibiliza os scripts '**test_pub.py**' e '**test_retrain.py**' para realização de testes para 
 verificar se alguns requisitos solicitados estão sendo atendidos. Também é possível criar testes personalizados através da 
 implementação da função '**test**' que se encontra nos scripts '**mytest_pub.py**' e '**mytest_retrain.py**'. Todos 
 estes scripts estão nas pastas **worker_pub** e **worker_retrain**.
```

### Comparing `mllibprodest-1.5.2/pyproject.toml` & `mllibprodest-1.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ['setuptools>=66.0.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mllibprodest"
-version = "1.5.2"
+version = "1.6.0"
 license = {text = "GPLv3"}
 authors = [
   { name="Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)", email="prodest@prodest.es.gov.br" },
 ]
 description = "Biblioteca de Machine Learning (ML) do Prodest."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: Portuguese (Brazilian)"
 ]
-dependencies = ['minio==7.1.14', 'python-dotenv==1.0.0', 'mlflow==2.3.2', 'boto3==1.26.134']
+dependencies = ['minio==7.1.15', 'python-dotenv==1.0.0', 'mlflow==2.5.0', 'boto3==1.28.21']
 keywords = ['Prodest', 'ML', 'lib', 'stack']
 
 [project.urls]
 "Homepage" = "https://github.com/prodest/mllibprodest"
 "Bug Tracker" = "https://github.com/prodest/mllibprodest/issues"
 "Documentation" = "https://prodest.github.io/mllibprodest"
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest/interfaces.py` & `mllibprodest-1.6.0/src/mllibprodest/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,43 @@
 class ModelPublicationInterfaceCLF(CommonMethods, metaclass=abc.ABCMeta):
     """
     Interface para publicação de modelos de ML com a função de classificação.
     Leia a documentação dos métodos e implemente-os seguindo as recomendações de tipos de parâmetros e retorno.
     """
     @classmethod
     def __subclasshook__(cls, subclass):
-        return (hasattr(subclass, 'predict') and
+        return (hasattr(subclass, 'get_model_name') and
+                callable(subclass.get_model_name) and
+                hasattr(subclass, 'get_model_provider_name') and
+                callable(subclass.get_model_provider_name) and
+                hasattr(subclass, 'predict') and
                 callable(subclass.predict) and
                 hasattr(subclass, 'evaluate') and
                 callable(subclass.evaluate) and
                 hasattr(subclass, 'get_model_info') and
                 callable(subclass.get_model_info) or
                 NotImplemented)
 
     @abc.abstractmethod
+    def get_model_name(self) -> str:
+        """
+        Obtém o nome do modelo que está em produção.
+            :return: Nome do modelo que está em produção.
+        """
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def get_model_provider_name(self) -> str:
+        """
+        Obtém o nome do provider que proverá o modelo que está em produção.
+            :return: Nome do provider que proverá o modelo que está em produção.
+        """
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def predict(self, dataset: list) -> list:
         """
         Faz predições utilizando o modelo que está em produção.
             :param dataset: Lista com os dados utilizados como features para realizar a predição.
             :return: Lista com os labels preditos.
         """
         raise NotImplementedError
@@ -79,40 +99,40 @@
                 hasattr(subclass, 'retrain') and
                 callable(subclass.retrain) or
                 NotImplemented)
 
     @abc.abstractmethod
     def get_model_name(self) -> str:
         """
-        Obtém o nome do modelo que estará em produção.
-            :return: Nome do modelo que estará em produção.
+        Obtém o nome do modelo que está em produção.
+            :return: Nome do modelo que está em produção.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_model_provider_name(self) -> str:
         """
-        Obtém o nome do provider que proverá o modelo que estará em produção.
-            :return: Nome do provider que proverá o modelo que estará em produção.
+        Obtém o nome do provider que proverá o modelo que está em produção.
+            :return: Nome do provider que proverá o modelo que está em produção.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_experiment_name(self) -> str:
         """
         Obtém o nome do experimento que será utilizado em produção.
             :return: Nome do experimento que será utilizado em produção.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_dataset_provider_name(self) -> str:
         """
-        Obtém o nome do provider do dataset usado pelo modelo que estará em produção.
-            :return: Nome do provider do dataset usado pelo modelo que estará em produção.
+        Obtém o nome do provider do dataset usado pelo modelo que está em produção.
+            :return: Nome do provider do dataset usado pelo modelo que está em produção.
         """
         raise NotImplementedError
 
     @staticmethod
     def generate_batch_indices(dataset_size: int, batch_size: int = 100000):
         """
         Gera indices para auxiliar na predição de registros em lote. Esta função gera uma lista contendo tuplas de
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest/provider.py` & `mllibprodest-1.6.0/src/mllibprodest/provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.2/src/mllibprodest/providers_types/local_provider.py` & `mllibprodest-1.6.0/src/mllibprodest/providers_types/local_provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.2/src/mllibprodest/providers_types/minio_provider.py` & `mllibprodest-1.6.0/src/mllibprodest/providers_types/minio_provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.2/src/mllibprodest/providers_types/mlflow_provider.py` & `mllibprodest-1.6.0/src/mllibprodest/providers_types/mlflow_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     Carrega o modelo que está em produção e baixa os artefatos necessários utilizando o MLflow.
         :param model_name: Nome do modelo que será carregado.
         :param artifacts_destination_path: Caminho local para onde os artefatos serão baixados.
         :return: Modelo carregado.
     """
     artefatos_obrigatorios = ["TrainingParams.pkl", "TrainingDatasetsNames.pkl", "BaselineMetrics.pkl"]
-    caminho_artefatos = Path(artifacts_destination_path)
+    caminho_artefatos = Path(artifacts_destination_path) / model_name
 
     # Antes de carregar o modelo, faz uma limpeza em alguns artefatos antigos. Obs.: Isso é necessário para evitar que,
     # caso o usuário esqueça de salvar um artefato obrigatório, seja carregado um artefato antigo salvo localmente.
     if artifacts_destination_path == "temp_area":
         rmtree(caminho_artefatos, ignore_errors=True)
     else:
         for artefato in artefatos_obrigatorios:
@@ -29,54 +29,54 @@
 
     try:
         Path.mkdir(caminho_artefatos, parents=True, exist_ok=True)
     except PermissionError:
         msg = f"Não foi possível criar a pasta de destino dos artefatos '{artifacts_destination_path}'. Permissão " \
               f"de escrita negada. Programa abortado!"
         logging.error(msg)
-        raise PermissionError(msg)
+        raise PermissionError(msg) from None
 
     stage = 'Production'
 
     # Carrega o modelo que está em produção
     try:
         modelo = mlflow.pyfunc.load_model(model_uri=f"models:/{model_name}/{stage}")
     except RestException:
         msg = f"O modelo '{model_name}' no estágio '{stage}' não foi encontrado. Programa abortado!"
         logging.error(msg)
-        raise RuntimeError(msg)
+        raise RuntimeError(msg) from None
     except MlflowException as e:
         msg = f"Não foi possível carregar o modelo '{model_name}'. Mensagem do MLFlow: '{e}'. Programa abortado!"
         logging.error(msg)
-        raise RuntimeError(msg)
+        raise RuntimeError(msg) from None
 
     # Baixa todos os artefatos com base no 'run_id' do modelo
     endereco_base_artefatos = f"runs:/{modelo.metadata.run_id}/"
 
     try:
         mlflow.artifacts.download_artifacts(artifact_uri=endereco_base_artefatos, dst_path=str(caminho_artefatos))
     except MlflowException as e:
         msg = f"Não foi possível carregar os artefatos no endereço '{endereco_base_artefatos}'. " \
               f"Mensagem do MLFlow: '{e}'. Programa abortado!"
         logging.error(msg)
-        raise RuntimeError(msg)
+        raise RuntimeError(msg) from None
 
     return modelo
 
 
 def load_production_params_mlflow(model_name: str) -> dict:
     """
     Carrega os parâmetros que foram utilizados para treinar o modelo que está em produção no MLflow.
         :param model_name: Nome do modelo que está em produção.
         :return: Dicionário contendo os parâmetros carregados.
     """
     modelo = load_model_mlflow(model_name, artifacts_destination_path='temp_area')
     logging.info(f"Utilizando os parâmetros de produção do modelo '{model_name}' (run_id: {modelo.metadata.run_id})")
     parametros = None
-    nome_arq = str(Path("temp_area") / "TrainingParams.pkl")
+    nome_arq = str(Path("temp_area") / model_name / "TrainingParams.pkl")
     arq = None
     msg = ""
 
     try:
         arq = open(nome_arq, 'rb')
     except FileNotFoundError:
         msg += f"O arquivo '{nome_arq}' não foi encontrado. "
@@ -107,15 +107,15 @@
     Carrega os nomes dos datasets que foram utilizados para treinar o modelo que está em produção no MLflow.
         :param model_name: Nome do modelo que está em produção.
         :return: Dicionário contendo os nomes dos datasets carregados.
     """
     modelo = load_model_mlflow(model_name, artifacts_destination_path='temp_area')
     logging.info(f"Utilizando os parâmetros de produção do modelo '{model_name}' (run_id: {modelo.metadata.run_id})")
     nomes_datasets = None
-    nome_arq = str(Path("temp_area") / "TrainingDatasetsNames.pkl")
+    nome_arq = str(Path("temp_area") / model_name / "TrainingDatasetsNames.pkl")
     arq = None
     msg = ""
 
     try:
         arq = open(nome_arq, 'rb')
     except FileNotFoundError:
         msg += f"O arquivo '{nome_arq}' não foi encontrado. "
@@ -147,15 +147,15 @@
     automatizada do modelo.
         :param model_name: Nome do modelo que está em produção.
         :return: Dicionário contendo as métricas de baseline.
     """
     modelo = load_model_mlflow(model_name, artifacts_destination_path='temp_area')
     logging.info(f"Utilizando o baseline de produção do modelo '{model_name}' (run_id: {modelo.metadata.run_id})")
     baseline = None
-    nome_arq = str(Path("temp_area") / "BaselineMetrics.pkl")
+    nome_arq = str(Path("temp_area") / model_name / "BaselineMetrics.pkl")
     arq = None
     msg = ""
 
     try:
         arq = open(nome_arq, 'rb')
     except FileNotFoundError:
         msg += f"O arquivo '{nome_arq}' não foi encontrado. "
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest/shared_classes.py` & `mllibprodest-1.6.0/src/mllibprodest/shared_classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 
 class CommonMethods:
     """
     Métodos comuns entre as interfaces dos modelos publicados.
     """
     @staticmethod
-    def make_log(path: str):
+    def make_log(filename: str):
         """
         Cria um arquivo para geração de logs. Se o mesmo já existir, inicia a gravação a partir do final desse arquivo.
         Depois de executar este método, para gravar os logs basta importar o pacote 'logging' e mandar salvar as
         mensagens de log com as funções: 'logging.error', 'logging.warning' ou 'logging.info', de acordo com o nível
         de criticidade da mensagem. Para mais opções, consulte a documentação do pacote 'logging'.
-            :param path: Caminho do arquivo de logs.
+            :param filename: Nome do arquivo de logs.
         """
-        make_log(path)
+        make_log(filename)
 
     @staticmethod
     def load_datasets(datasets_filenames: dict, provider: str = 'minio') -> dict:
         """
         Carrega os datasets necessários para o modelo. Os parâmetros de acesso deverão ser fornecidos através de um
         arquivo chamado '.env' que deve ser criado no repositório local e preenchido com as seguintes variáveis:
         MINIO = "nome do servidor s3", ACCESS_KEY = "chave de acesso", SECRET_KEY = "senha de acesso" e
@@ -89,68 +89,71 @@
             :param artifacts_destination_path: Caminho para onde os artefatos serão baixados.
             :return: Modelo carregado.
         """
         return Provider.load_model(model_name=model_name, provider=provider,
                                    artifacts_destination_path=artifacts_destination_path)
 
     @staticmethod
-    def convert_artifact_to_pickle(artifact: object, file_name: str, path: str = "temp_area"):
+    def convert_artifact_to_pickle(model_name: str, artifact: object, file_name: str, path: str = "temp_area"):
         """
         Converte um artefato para o formato pickle, para facilitar a persistência.
+            :param model_name: Nome do modelo em que o artefato será utilizado.
             :param artifact: Artefato que será convertido (str, list, dict, tuple, etc.).
             :param file_name: Nome do arquivo que será gerado (Dica: Use a extensão '.pkl').
             :param path: Caminho para gerar o artefato convertido.
         """
-        caminho_artefato = str(Path(path) / file_name)
+        caminho_artefato = str(Path(path) / model_name / file_name)
 
         try:
             arq = open(caminho_artefato, 'wb')
         except FileNotFoundError:
             msg = f"Não foi possível gerar o artefato '{file_name}' convertido. O caminho '{caminho_artefato}' está " \
                   f"incorreto. Programa abortado!"
             logging.error(msg)
-            raise FileNotFoundError(msg)
+            raise FileNotFoundError(msg) from None
         except PermissionError:
-            msg = f"Não foi possível gerar o artefato '{file_name}' convertido no caminho '{path}'. Permissão de " \
-                  f"escrita negada. Programa abortado!"
+            msg = f"Não foi possível gerar o artefato '{file_name}' convertido no caminho '{caminho_artefato}'. " \
+                  f"Permissão de escrita negada. Programa abortado!"
             logging.error(msg)
-            raise PermissionError(msg)
+            raise PermissionError(msg) from None
 
         try:
             pickle.dump(artifact, arq)
         except TypeError as e:
             msg = f"Não foi possível gerar o artefato '{file_name}' com o Pickle (mensagem Pickle: {e}). Programa " \
                   f"abortado!"
             logging.error(msg)
-            raise TypeError(msg)
+            raise TypeError(msg) from None
 
         arq.close()
 
     @staticmethod
-    def convert_artifact_to_object(file_name: str, path: str = "temp_area") -> Union[list, tuple, dict, object]:
+    def convert_artifact_to_object(model_name: str, file_name: str, path: str = "temp_area") -> \
+            Union[list, tuple, dict, object]:
         """
         Converte um artefato que está no formato pickle para o objeto de origem.
+            :param model_name: Nome do modelo ao qual o artefato pertence.
             :param file_name: Nome do arquivo que será lido e convertido.
             :param path: Caminho onde o arquivo a ser convertido se encontra.
             :return: Artefato convertido.
         """
-        caminho_artefato = str(Path(path) / file_name)
+        caminho_artefato = str(Path(path) / model_name / file_name)
 
         try:
             arq = open(caminho_artefato, 'rb')
         except FileNotFoundError:
             msg = f"Não foi possível converter o artefato '{file_name}'. O caminho '{caminho_artefato}' não foi " \
                   f"encontrado. Programa abortado!"
             logging.error(msg)
-            raise FileNotFoundError(msg)
+            raise FileNotFoundError(msg) from None
         except PermissionError:
-            msg = f"Não foi possível converter o artefato '{file_name}' usando o caminho '{path}'. Permissão de " \
-                  f"leitura negada. Programa abortado!"
+            msg = f"Não foi possível converter o artefato '{file_name}' usando o caminho '{caminho_artefato}'. " \
+                  f"Permissão de leitura negada. Programa abortado!"
             logging.error(msg)
-            raise PermissionError(msg)
+            raise PermissionError(msg) from None
 
         try:
             objeto = pickle.load(arq)
         except pickle.UnpicklingError as e:
             msg = f"Não foi possível converter o artefato '{file_name}' com o Pickle (mensagem Pickle: {e}). " \
                   f"Programa abortado!"
             logging.error(msg)
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest/validators/test.py` & `mllibprodest-1.6.0/src/mllibprodest/validators/test.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,391 +6,355 @@
 import logging
 import hashlib
 import time
 import os
 from pathlib import Path
 from shutil import copytree, rmtree
 from ..utils import make_log
+from ..initiators.model_initiator import InitModels
 
+# Códigos para impressão de mensagens coloridas no terminal
+BLUE = "\033[1;34m"
+RED = "\033[1;31m"
+GREEN = "\033[0;32m"
+BOLD = "\033[;1m"
+RESET = "\033[0;0m"
 
 class Test:
     """
     Classe para realização de testes para validação da implementação das interfaces da lib. Obs.: Não tem nada a ver
     com 'Unit testing framework' (https://docs.python.org/3/library/unittest.html).
     """
     def __init__(self):
         make_log("log_tests.log")
 
         h = hashlib.md5()
         h.update(str(time.time()).encode())
-        self._test_id = h.hexdigest()
+        self.__test_id = h.hexdigest()
 
-        msg = f"------------------> Instanciando o teste com o ID: {self._test_id} <------------------"
+        msg = f"------------------> Instanciando o teste com o ID: {self.__test_id} <------------------"
         logging.info(msg)
-        print(f"\n\n{msg}")
+        print(f"\n\n      {BOLD}{BLUE}{msg}{RESET}")
 
         pasta_corrente = Path.cwd().name
 
         if pasta_corrente == "worker_pub":
-            if Path.exists(Path("pub.py")):
-                self.__nome_pasta_worker = "worker_pub"
-                self._nome_script = "pub.py"
-                self._nome_mytest = "mytest_pub.py"
-            else:
-                msg = "O arquivo 'pub.py' não foi encontrado na pasta 'worker_pub'. Por favor, crie o script " \
-                      "'pub.py' dentro da pasta 'worker_pub' e construa uma classe chamada 'ModeloCLF' que " \
-                      "implementa a interface 'ModelPublicationInterfaceCLF'. Teste abortado!"
-                logging.error(msg)
-                print(f"\n\n{msg}")
-                exit(1)
+            self.__nome_pasta_worker = "worker_pub"
+            self.__nome_mytest = "mytest_pub.py"
         elif pasta_corrente == "worker_retrain":
-            if Path.exists(Path("retrain.py")):
-                self.__nome_pasta_worker = "worker_retrain"
-                self._nome_script = "retrain.py"
-                self._nome_mytest = "mytest_retrain.py"
-            else:
-                msg = "O arquivo 'retrain.py' não foi encontrado na pasta 'worker_retrain'. Por favor, crie o script " \
-                      "'retrain.py' dentro da pasta 'worker_retrain' e construa uma classe chamada 'ModeloRETRAIN' " \
-                      "que implementa a interface 'ModelPublicationInterfaceRETRAIN'. Teste abortado!"
-                logging.error(msg)
-                print(f"\n\n{msg}")
-                exit(1)
+            self.__nome_pasta_worker = "worker_retrain"
+            self.__nome_mytest = "mytest_retrain.py"
         else:
             msg = "Não foi possível encontrar a pasta 'worker_pub' ou 'worker_retrain'. Verifique se estas pastas " \
                   "existem ou se você está rodando os testes na pasta correta. Teste abortado!"
             logging.error(msg)
             print(f"\n\n{msg}")
+            print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
             exit(1)
 
-        msg = f"O script '{self._nome_script}' foi encontrado!"
-        logging.info(msg)
-        print(f"\n\n{msg}")
-
         if Path.exists(Path("requirements.txt")):
-            arq = None
-
             try:
                 arq = open("requirements.txt", "r")
             except PermissionError:
                 msg = f"Não foi possível ler o arquivo 'requirements.txt' dentro da pasta " \
                       f"'{self.__nome_pasta_worker}'. Permissão de leitura negada. Teste abortado!"
                 logging.error(msg)
                 print(f"\n\n{msg}")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
 
             reqs = arq.readlines()
             arq.close()
             vazio = True
 
             for r in reqs:
                 linha = r.rstrip('\n')
 
                 if len(linha) >= 1:
                     vazio = False
                     break
 
             if not vazio:
-                msg = f"O arquivo 'requirements.txt' foi encontrado na pasta '{self.__nome_pasta_worker}' e não " \
+                msg = f"O arquivo 'requirements.txt' foi encontrado na pasta '{self.__nome_pasta_worker}' e NÃO " \
                       f"está vazio!"
                 logging.info(msg)
                 print(f"\n\n{msg}")
             else:
                 msg = f"O arquivo 'requirements.txt' foi encontrado na pasta '{self.__nome_pasta_worker}' mas está " \
                       f"vazio. Teste abortado!"
                 logging.error(msg)
                 print(f"\n\n{msg}")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
         else:
             msg = f"O arquivo 'requirements.txt' não foi encontrado na pasta '{self.__nome_pasta_worker}'. Por favor," \
-                  f" gere este arquivo com a lista de pacotes que foram utilizados na construção do script " \
-                  f"'{self._nome_script}'. Teste abortado!"
+                  f" gere este arquivo com a lista de pacotes que foram utilizados na construção do(s) modelo(s). " \
+                  f"Teste abortado!"
             logging.error(msg)
             print(f"\n\n{msg}")
+            print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
             exit(1)
 
         # Howto para informar como passar uma função personalizada para realização dos testes
-        self._howto_msg = f"1. Edite o script '{self._nome_mytest}' (está na pasta '{self.__nome_pasta_worker}')" \
-                          f" para implementar a função 'test()';\n2. Crie os testes adicionais que você julgar " \
-                          f"necessários para testar o código do worker.\n   REGRAS: Esta função não deve receber " \
-                          f"parâmetros e retornar nada. Todos os dados para rodá-la devem ser obtidos de dentro " \
-                          f"dela.\n   A responsabilidade de criar os testes personalizados e verificar se passaram " \
-                          f"é do desenvolvedor do modelo."
+        self.__howto_msg = f"1. Edite o script '{self.__nome_mytest}' (está na pasta '{self.__nome_pasta_worker}')" \
+                           f" para implementar a função 'test()';\n2. Crie os testes adicionais que você julgar " \
+                           f"necessários para testar o código do worker.\n   REGRAS: Esta função não deve receber " \
+                           f"parâmetros adicionais. Não pode retornar valores. Todos os dados para rodá-la devem ser " \
+                           f"obtidos de dentro dela.\n   A responsabilidade de criar os testes personalizados e " \
+                           f"verificar se passaram é do desenvolvedor do modelo."
 
         # Artefatos obrigatórios que devem ter os tipos de valores de retorno testados
-        self.mandatory_artifacts = {
+        self.__mandatory_artifacts = {
             'TrainingParams.pkl': dict,
             'TrainingDatasetsNames.pkl': dict,
             'BaselineMetrics.pkl': dict
         }
 
         # Métodos que devem ter os tipos de valores de retorno testados
-        self.methods_to_test = {
+        self.__methods_to_test = {
             'ModeloCLF': {
+                'ModeloCLF.get_model_name': str,
+                'ModeloCLF.get_model_provider_name': str,
                 'ModeloCLF.get_model_info': dict
             },
             'ModeloRETRAIN': {
                 'ModeloRETRAIN.get_model_name': str,
                 'ModeloRETRAIN.get_model_provider_name': str,
                 'ModeloRETRAIN.get_experiment_name': str,
                 'ModeloRETRAIN.get_dataset_provider_name': str
             }
         }
+
+        # Guarda os modelos instanciados
+        self.__modelos = None
+
+        # Instancia os scripts de testes personalizados
         self.__validation_function = None
 
-        if Path.exists(Path(self._nome_mytest)):
+        if Path.exists(Path(self.__nome_mytest)):
             try:
-                if self._nome_mytest == "mytest_pub.py":
+                if self.__nome_mytest == "mytest_pub.py":
                     from mytest_pub import test
                     self.__validation_function = test
-                elif self._nome_mytest == "mytest_retrain.py":
+                elif self.__nome_mytest == "mytest_retrain.py":
                     from mytest_retrain import test
                     self.__validation_function = test
             except ImportError:
                 msg = "AVISO: A função para realização do teste personalizado pelo usuário não foi encontrada." \
                       "\n       Caso deseje criar um teste personalizado, faça o seguinte:\n"
-                logging.info(msg + self._howto_msg)
-                print(f"\n\n{msg + self._howto_msg}\n")
+                logging.info(msg + self.__howto_msg)
+                print(f"\n\n{msg + self.__howto_msg}\n")
         else:
-            msg = f"AVISO: O arquivo '{self._nome_mytest}' não foi encontrado na pasta '{self.__nome_pasta_worker}'. " \
-                  f"Caso deseje criar um teste personalizado, crie\n       um arquivo chamado '{self._nome_mytest}' " \
-                  f"e faça o seguinte:\n"
-            logging.info(msg + self._howto_msg)
-            print(f"\n\n{msg + self._howto_msg}\n")
+            msg = f"AVISO: O arquivo '{self.__nome_mytest}' não foi encontrado na pasta '{self.__nome_pasta_worker}'" \
+                  f". Caso deseje criar um teste personalizado, crie\n       um arquivo chamado " \
+                  f"'{self.__nome_mytest}' e faça o seguinte:\n"
+            logging.info(msg + self.__howto_msg)
+            print(f"\n\n{msg + self.__howto_msg}\n")
 
     def __validate_methods(self, model, class_name: str) -> bool:
         """
-        Valida os métodos definidos no construtor da classe através do atributo 'self.methods_to_test'.
+        Valida os métodos definidos no construtor da classe através do atributo 'self.__methods_to_test'.
             :param model: Modelo de onde os métodos serão chamados.
             :param class_name: Nome da classe que possui os métodos que serão validados.
             :return: True, se todos os métodos foram validados. False, caso algum método não tenha sido validado.
         """
         validado = True
 
-        for method_name, return_type in self.methods_to_test[class_name].items():
+        for method_name, return_type in self.__methods_to_test[class_name].items():
             nome_metodo_aux = method_name.split(".")[1]
-            msg = f"Testando o método '{nome_metodo_aux}'..."
+            msg = f"=> Testando o método '{nome_metodo_aux}'..."
             logging.info(msg)
             print(f"\n\n{msg}\n")
 
             retorno = None
 
             try:
-                if method_name == "ModeloCLF.get_model_info":
+                if method_name == "ModeloCLF.get_model_name":
+                    retorno = model.get_model_name()
+                elif method_name == "ModeloCLF.get_model_provider_name":
+                    retorno = model.get_model_provider_name()
+                elif method_name == "ModeloCLF.get_model_info":
                     retorno = model.get_model_info()
                 elif method_name == "ModeloRETRAIN.get_model_name":
                     retorno = model.get_model_name()
                 elif method_name == "ModeloRETRAIN.get_model_provider_name":
                     retorno = model.get_model_provider_name()
                 elif method_name == "ModeloRETRAIN.get_experiment_name":
                     retorno = model.get_experiment_name()
                 elif method_name == "ModeloRETRAIN.get_dataset_provider_name":
                     retorno = model.get_dataset_provider_name()
             except AttributeError as e:
                 msg = f"A chamada ao método '{nome_metodo_aux}' falhou: {str(e)}."
                 logging.error(msg)
-                print(f"\n\n{msg}\n")
+                print(f"\n{RED}***ERRO***: {msg}{RESET}\n")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
 
             tipo_retorno = type(retorno)
 
             if tipo_retorno is return_type:
                 msg = f"Tipo de retorno da chamada ao método '{nome_metodo_aux}' OK: {retorno}"
                 logging.info(msg)
-                print(f"\n\n{msg}\n")
+                print(f"   {msg}\n")
             else:
                 validado = False
                 msg = f"O método '{nome_metodo_aux}' deve retornar o tipo '{return_type.__name__}', porém retornou " \
                       f"'{tipo_retorno.__name__}'."
                 logging.error(msg)
-                print(f"\n\n{msg}\n")
+                print(f"{RED}***ERRO***: {msg}{RESET}\n")
 
         return validado
 
     def __validate_mandatory_artifacts(self, model) -> bool:
         """
         Valida se os artefatos obrigatórios definidos para o modelo foram implementados pelo usuário.
             :param model: Modelo de onde será chamada a função utilitária 'convert_artifact_to_object'.
             :return: True, se todos os artefatos obrigatórios foram encontrados. False, caso algum artefato obrigatório
                      não tenha sido encontrado.
         """
         validado = True
 
-        for nome_artefato_obrigatorio, tipo_artefato_obrigatorio in self.mandatory_artifacts.items():
-            msg = f"Procurando pelo artefato obrigatório '{nome_artefato_obrigatorio}'..."
+        for nome_artefato_obrigatorio, tipo_artefato_obrigatorio in self.__mandatory_artifacts.items():
+            msg = f"=> Procurando pelo artefato obrigatório '{nome_artefato_obrigatorio}'..."
             logging.info(msg)
-            print(f"\n\n{msg}\n")
+            print(f"\n{msg}\n")
 
-            artefato_lido = model.convert_artifact_to_object(file_name=nome_artefato_obrigatorio)
+            artefato_lido = model.convert_artifact_to_object(model_name=model.get_model_name(),
+                                                             file_name=nome_artefato_obrigatorio)
             tipo_artefato_lido = type(artefato_lido)
 
             if tipo_artefato_lido is tipo_artefato_obrigatorio:
                 if len(artefato_lido) > 0:
                     msg = f"Conteúdo do artefato obrigatório '{nome_artefato_obrigatorio}': '{artefato_lido}'"
                     logging.info(msg)
-                    print(f"\n\n{msg}\n")
+                    print(f"  {msg}\n")
                 else:
                     validado = False
                     msg = f"O artefato obrigatório '{nome_artefato_obrigatorio}' deve ter o tamanho maior que 0 (zero)."
                     logging.error(msg)
-                    print(f"\n\n{msg}\n")
+                    print(f"{RED}***ERRO***: {msg}{RESET}\n")
             else:
                 validado = False
                 msg = f"O artefato obrigatório '{nome_artefato_obrigatorio}' deve ser do tipo " \
                       f"'{tipo_artefato_obrigatorio.__name__}', porém é do tipo: '{tipo_artefato_lido.__name__}'."
                 logging.error(msg)
-                print(f"\n\n{msg}\n")
+                print(f"{RED}***ERRO***: {msg}{RESET}\n")
 
         return validado
 
     def __validate_pub(self):
         """
-        Valida o script pub.py.
+        Valida os scripts para publicação do modelo utilizando a classe ModeloCLF.
         """
-        modelo_teste = None
-        msg = "Importando a classe 'ModeloCLF'..."
+        msg = "Scripts para publicação do modelo utilizando a classe 'ModeloCLF'..."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
-
-        try:
-            from pub import ModeloCLF
-        except ImportError:
-            msg = "A definição da classe 'ModeloCLF' não foi encontrada no arquivo 'pub.py'."
-            logging.error(msg)
-            print(f"\n\n{msg}\n")
-            exit(1)
+        print(f"\n\n # {msg}")
 
-        msg = "Instanciando um objeto da classe 'ModeloCLF'..."
-        logging.info(msg)
-        print(f"\n\n{msg}\n")
+        for nome_modelo, modelo in self.__modelos.items():
+            print(f"\n{GREEN} ### MODELO: {nome_modelo} ### {RESET}\n")
 
-        if callable(ModeloCLF) and type(ModeloCLF).__name__ == 'ABCMeta':
-            try:
-                modelo_teste = ModeloCLF()
-            except TypeError as e:
-                msg = f"Faltou a implementação do(s) seguinte(s) método(s): {str(e)[65:]}."
+            if not self.__validate_methods(modelo, "ModeloCLF"):
+                msg = "Erro ao validar os métodos obrigatórios. Verifique as mensagens de validação acima."
                 logging.error(msg)
-                print(f"\n\n{msg}\n")
+                print(f"\n\n{RED} *** {msg}{RESET}\n")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
 
-            msg = "AVISO: Os métodos 'predict' e 'evaluate' não serão testados porque necessitam de dados que são " \
-                  "específicos para cada implementação.\nCaso deseje testar estes métodos, faça o seguinte:\n"
-            logging.info(msg + self._howto_msg)
-            print(f"\n\n{msg + self._howto_msg}\n")
+        msg = "AVISO: Os métodos 'predict' e 'evaluate' não serão testados porque necessitam de dados que " \
+              "são específicos para cada implementação.\nCaso deseje testar estes métodos, faça o seguinte:\n"
+        logging.info(msg + self.__howto_msg)
+        print(f"\n\n{msg + self.__howto_msg}\n")
 
-            if not self.__validate_methods(modelo_teste, "ModeloCLF"):
-                exit(1)
-        else:
-            msg = f"O tipo do 'ModeloCLF' está incorreto: '{type(ModeloCLF).__name__}'. 'ModeloCLF' deve ser uma " \
-                  f"classe que herda os métodos da interface 'ModelPublicationInterfaceCLF' e possua as " \
-                  f"implementações para os métodos abstratos dela."
-            logging.error(msg)
-            print(f"\n\n{msg}\n")
-            exit(1)
 
     def __validate_retrain(self):
         """
-        Valida o script retrain.py.
+        Valida os scripts para publicação do modelo utilizando a classe ModeloRETRAIN.
         """
-        modelo_teste = None
-        msg = "Importando a classe 'ModeloRETRAIN'..."
+        msg = "Scripts para publicação do modelo utilizando a classe 'ModeloRETRAIN'..."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
-
-        try:
-            from retrain import ModeloRETRAIN
-        except ImportError:
-            msg = "A definição da classe 'ModeloRETRAIN' não foi encontrada no arquivo 'retrain.py'."
-            logging.error(msg)
-            print(f"\n\n{msg}\n")
-            exit(1)
+        print(f"\n\n # {msg}")
 
-        msg = "Instanciando um objeto da classe 'ModeloRETRAIN'..."
-        logging.info(msg)
-        print(f"\n\n{msg}\n")
+        for nome_modelo, modelo in self.__modelos.items():
+            print(f"\n{GREEN} ### MODELO: {nome_modelo} ### {RESET}\n")
 
-        if callable(ModeloRETRAIN) and type(ModeloRETRAIN).__name__ == 'ABCMeta':
-            try:
-                modelo_teste = ModeloRETRAIN()
-            except TypeError as e:
-                msg = f"Faltou a implementação do(s) seguinte(s) método(s): {str(e)[65:]}."
+            if not self.__validate_methods(modelo, "ModeloRETRAIN"):
+                msg = "Erro ao validar os métodos obrigatórios. Verifique as mensagens de validação acima."
                 logging.error(msg)
-                print(f"\n\n{msg}\n")
-                exit(1)
-
-            msg = "AVISO: Os métodos 'evaluate' e 'retrain' não serão testados porque necessitam de dados que são " \
-                  "específicos para cada implementação.\nCaso deseje testar estes métodos, faça o seguinte:\n"
-            logging.info(msg + self._howto_msg)
-            print(f"\n\n{msg + self._howto_msg}\n")
-
-            if not self.__validate_methods(modelo_teste, "ModeloRETRAIN"):
+                print(f"\n\n{RED} *** {msg}{RESET}\n")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
 
             # Testa o carregamento do modelo e verifica se os artefatos obrigatórios estão de acordo
-            model_name = modelo_teste.get_model_name()
-            provider_name = modelo_teste.get_model_provider_name()
+            model_name = modelo.get_model_name()
+            provider_name = modelo.get_model_provider_name()
 
             try:
-                modelo_teste.load_model(model_name=model_name, provider=provider_name)
+                modelo.load_model(model_name=model_name, provider=provider_name)
             except AttributeError as e:
                 msg = f"A chamada ao método 'load_model' falhou: {str(e)}."
                 logging.error(msg)
                 print(f"\n\n{msg}\n")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
 
-            if not self.__validate_mandatory_artifacts(modelo_teste):
+            if not self.__validate_mandatory_artifacts(modelo):
+                msg = "Erro ao validar os artefatos obrigatórios. Verifique as mensagens de validação acima."
+                logging.error(msg)
+                print(f"\n\n{RED} *** {msg}{RESET}\n")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
-        else:
-            msg = f"O tipo do 'ModeloRETRAIN' está incorreto: '{type(ModeloRETRAIN).__name__}'. 'ModeloRETRAIN' deve " \
-                  f"ser uma classe que herda os métodos da interface 'ModelPublicationInterfaceRETRAIN' e possua as " \
-                  f"implementações para os métodos abstratos dela."
-            logging.error(msg)
-            print(f"\n\n{msg}\n")
-            exit(1)
+
+        msg = "AVISO: Os métodos 'evaluate' e 'retrain' não serão testados porque necessitam de dados que " \
+              "são específicos para cada implementação.\nCaso deseje testar estes métodos, faça o seguinte:\n"
+        logging.info(msg + self.__howto_msg)
+        print(f"\n\n{msg + self.__howto_msg}\n")
 
     def __validate_params_returns(self):
         """
         Valida alguns parâmetros e valores de retorno solicitados pelas interfaces que foram implementados. Porém, não
         é escopo desta função validar os dados que estão sendo utilizados pelas funções implementadas.
         """
-        msg = f"=> INICIO: Test ID={self._test_id}. Teste padrão da lib."
+        msg = f"=> INICIO: Test ID={self.__test_id}. Teste padrão da lib."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
+        print(f"\n\n{BOLD}{BLUE}{msg}{RESET}\n")
 
-        if self._nome_script == "pub.py":
+        if self.__nome_pasta_worker == "worker_pub":
             self.__validate_pub()
-        elif self._nome_script == "retrain.py":
+        elif self.__nome_pasta_worker == "worker_retrain":
             self.__validate_retrain()
 
-        msg = f"=> FIM: Test ID={self._test_id}. Teste padrão da lib."
+        msg = f"=> FIM: Test ID={self.__test_id}. Teste padrão da lib."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
+        print(f"\n\n{BOLD}{BLUE}{msg}{RESET}\n")
 
     def __run_validation_function(self):
         """
         Executa a função de validação criada e personalizada pelo usuário.
         """
-        msg = f"=> INICIO: Test ID={self._test_id}. Testes personalizados pelo usuário. Dados da função utilizada: " \
+        msg = f"=> INICIO: Test ID={self.__test_id}. Testes personalizados pelo usuário. Dados da função utilizada: " \
               f"{str(self.__validation_function)}."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
+        print(f"\n\n{BOLD}{BLUE}{msg}{RESET}\n")
 
         type_validation_function = type(self.__validation_function).__name__
 
         if type_validation_function != 'function':
             msg = f"O parâmetro 'validation_function' deve receber uma função mas recebeu " \
-                  f"'{type_validation_function}'."
+                  f"'{type_validation_function}'. Verifique a implementação da função 'test' no arquivo " \
+                  f"'{self.__nome_mytest}'."
             logging.error(msg)
             print(f"\n\n{msg}")
+            print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
             exit(1)
 
-        self.__validation_function()
+        self.__validation_function(self.__modelos)
 
-        msg = f"=> FIM: Test ID={self._test_id}. Testes personalizados pelo usuário."
+        msg = f"=> FIM: Test ID={self.__test_id}. Testes personalizados pelo usuário."
         logging.info(msg)
-        print(f"\n\n{msg}\n")
+        print(f"\n\n{BOLD}{BLUE}{msg}{RESET}\n")
 
     def validate(self, mlruns_path: str = ""):
         """
         Valida a implementação das interfaces da lib através das chamadas de funções específicas para este fim. Além do
         conjunto de testes padrões executados pela lib, se os arquivos 'mytest_pub.py' e 'mytest_retrain.py' existirem
         nas pastas de cada worker respectivamente, a função 'test()' será procurada e, caso exista, será carregada e
         utilizada para rodar os testes personalizados pelo usuário.
@@ -411,24 +375,33 @@
 
                 try:
                     copytree(caminho_mlruns, "mlruns", dirs_exist_ok=True)
                 except FileNotFoundError:
                     msg = "O caminho para a pasta 'mlruns' está incorreto. Teste abortado!"
                     logging.error(msg)
                     print(f"\n\n{msg}")
+                    print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                     exit(1)
                 except PermissionError:
                     msg = f"Permissão de leitura na pasta de origem ('{caminho_mlruns}') ou gravação na pasta de " \
                           f"destino ('mlruns') negada. Teste abortado!"
                     logging.error(msg)
                     print(f"\n\n{msg}")
+                    print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                     exit(1)
 
                 os.environ["MLFLOW_TRACKING_URI"] = "http://localhost:5000"
 
+                msg = "=> Instanciando os modelos definidos no arquivo 'params.conf'..."
+                logging.info(msg)
+                print(f"\n\n{msg}\n")
+
+                # Não tratei as exceções para preservar o traceback e facilitar a procura da origem do erro.
+                self.__modelos = InitModels.init_models()
+
                 # Roda os testes padrões da lib
                 self.__validate_params_returns()
 
                 # Se foi criada uma função para o teste, utiliza
                 if self.__validation_function is not None:
                     self.__run_validation_function()
 
@@ -436,14 +409,15 @@
                 try:
                     copytree("mlruns", caminho_mlruns, dirs_exist_ok=True)
                 except PermissionError:
                     msg = f"Permissão de leitura na pasta de origem ('mlruns') ou gravação na pasta de destino " \
                           f"('{caminho_mlruns}') negada. Teste abortado!"
                     logging.error(msg)
                     print(f"\n\n{msg}")
+                    print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                     exit(1)
 
                 # Limpa os arquivos criados na execução dos testes
                 for path in Path("temp_area").glob("**/*"):
                     if path.is_file():
                         path.unlink()
                     elif path.is_dir():
@@ -452,13 +426,21 @@
                 rmtree("mlruns", ignore_errors=True)
             else:
                 msg = "Informe o parâmetro '--mlruns_path=<caminho completo para a pasta mlruns>' ao rodar o script. " \
                       "A pasta 'mlruns' é criada na pasta local onde o servidor do MLflow, utilizado para registrar " \
                       "o modelo, foi iniciado. Teste abortado!"
                 logging.error(msg)
                 print(f"\n\n{msg}")
+                print(f"\n{RED}  *** O TESTE FALHOU! ***{RESET}\n")
                 exit(1)
         else:  # Encontrou as variáveis de ambiente e vai rodar com o MLflow remoto
+            msg = "=> Instanciando os modelos definidos no arquivo 'params.conf'..."
+            logging.info(msg)
+            print(f"\n\n{msg}\n")
+
+            # Não tratei as exceções para preservar o traceback e facilitar a procura da origem do erro.
+            self.__modelos = InitModels.init_models()
+
             self.__validate_params_returns()
 
             if self.__validation_function is not None:
                 self.__run_validation_function()
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest.egg-info/PKG-INFO` & `mllibprodest-1.6.0/src/mllibprodest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.5.2
+Version: 1.6.0
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
@@ -73,15 +73,15 @@
 # Obs.: Utilize as duas linhas abaixo, exatamente como apresentadas, para configurar o parâmetro 'Tracking URI' do MLflow 
 # nos seus códigos de testes. Dessa forma, quando subir para produção não haverá necessidade de modificá-las, pois lá
 # o parâmetro 'Tracking URI' será obtido diretamente através da variável de ambiente 'MLFLOW_TRACKING_URI'.
 if os.environ.get('MLFLOW_TRACKING_URI') is None:
     mlflow.set_tracking_uri('sqlite:///teste_mlflow.db')
 
 # Configura o experimento (se não existir, cria)
-mlflow.set_experiment(experiment_name="Teste sklearn")
+mlflow.set_experiment(experiment_name="Teste_sklearn")
 
 # Inicia uma execução do experimento (um experimento pode possuir várias execuções)
 mlflow.start_run(run_name="t1", description="teste 1")
 
 # Registra algumas informações adicionais no experimento (coloque as informações que julgar necessárias, no formato dict)
 tags = {"Projeto": "Teste", "team": "ML", "util": "Informação útil"}
 mlflow.set_tags(tags)
@@ -128,28 +128,28 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
+pip install mlflow==2.5.0 scikit-learn==1.3.0 matplotlib==3.7.2 numpy==1.25.2
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
 Abaixo segue uma listagem do conteúdo gerado pelo código de teste (obs.: essa parte do caminho vai ser diferente de 
-acordo com cada experimento/execução realizados: '1/f454220e01bd43e7b66c2354c20f0085'. O conteúdo da pasta também será 
+acordo com cada experimento/execução realizados: '1/9d01359d68034063867613196395388e'. O conteúdo da pasta também será 
 diferente de acordo com cada modelo).
 ```bash
-(env) user:~/testes/mlruns/1/f454220e01bd43e7b66c2354c20f0085/artifacts$ dir
-artefato.pkl  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
+(env) user:~/testes/mlruns/1/9d01359d68034063867613196395388e/artifacts$ dir
+artefato.pkl  estimator.html  model  training_confusion_matrix.png  training_precision_recall_curve.png  training_roc_curve.png
 ```
 Dentro da pasta criada para testes também foi gerado um arquivo chamado '**teste_mlflow.db**', que é um pequeno banco 
 de dados [SQlite](https://www.sqlite.org), que serve para armazenar os modelos que foram registrados.
 
 - Inicie o servidor do MLflow;
 
 Perceba que a pasta '**mlruns**' e o arquivo '**teste_mlflow.db**' foram passados como parâmetros na hora de iniciar o 
@@ -159,16 +159,16 @@
 **DICA**: Abra um outro prompt de comando ou terminal diferente; entre na pasta onde se encontra o código para registro 
 dos experimentos/modelo; execute o comando para iniciar o servidor do MLflow de dentro desta pasta. Pois assim, você 
 conseguirá rodar o código e já observar os resultados sem ter que parar o servidor para liberar o prompt ou terminal.
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 
-- Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
-pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
+- Verifique se o experimento foi criado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
+pelo experimento/execução '**Teste_sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
 - Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
@@ -211,19 +211,18 @@
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja 
 possível carregar o modelo.
 
 ## 2. Organize o código de acordo com o *template*
 Uma vez que o modelo foi desenvolvido e testado, agora é o momento de iniciar as tratativas para publicá-lo na *stack* de ML do 
-Prodest. Porém, antes, é oporturno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
+Prodest. Porém, antes, é oportuno mostrar como o modelo será integrado à *stack*. Esta integração se dará através de 
 componentes denominados *workers*, cuja codificação é de responsabilidade de quem está construindo o modelo. Na 
 ilustração abaixo é possível observar que os *workers* são acessados pelos componentes de apoio da *stack* para 
-permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo, desde que 
-sejam construídos *workers* dedicados para cada um deles.
+permitir a publicação dos modelos. Caso seja necessário, uma mesma stack poderá publicar mais de um modelo.
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/stack-ml.png?raw=true)
 
 Existem dois tipos de *workers*:
 - **worker_pub**: Fornece os métodos necessários para publicação do modelo.
 - **worker_retrain**: Responsável pela avaliação do desempenho do modelo e retreinamento, se for preciso.
 
@@ -294,19 +293,19 @@
 *workers*. Dessa forma, à medida que você for produzindo o código e necessitar de instalar pacotes, esses serão 
 instalados nos ambientes virtuais criados. Quando terminar a implementação, basta você gerar os arquivos de 
 *requirements* com base no ambiente virtual de cada *worker* separadamente. Acredite, isso vai te ajudar bastante!
 
 Outro ponto importante antes de implementar as interfaces é saber que: para publicar o modelo será necessário a criação 
 de três artefatos obrigatórios, inclusive seguindo o mesmo nome (*case sensitive*). Estes artefatos devem ser 
 dicionários (dict) salvos com o [Pickle](https://docs.python.org/3/library/pickle.html) (utilize a função 
-'convert_artifact_to_pickle' quando estiver implementando as intefaces):
+'convert_artifact_to_pickle' quando estiver implementando as interfaces):
 
 - **TrainingParams.pkl**: Deve conter os parâmetros que você escolheu utilizar no treinamento do modelo. Não há 
-necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros 
-criados por você necessários para que o modelo funcione. Coloque o nome 
+necessidade de colocar os parâmetros nos quais você manteve os valores *default*. Você pode colocar outros parâmetros, 
+criados por você, necessários para que o modelo funcione. Coloque o nome 
 do parâmetro como nome da chave e o valor do parâmetro como valor da chave. Ex. baseado no *DecisionTreeClassifier*: 
 {'criterion': 'entropy', 'max_depth': '20', 'random_state': '77', 'meu_parametro_personalizado': 'teste'}. 
 
 
 - **TrainingDatasetsNames.pkl**: Deve conter os tipos de datasets e os nomes dos respectivos arquivos utilizados no
 treinamento do modelo. Exemplo: {'features': 'nome_arquivo_features', 'targets': 'nome_arquivo_targets'}.
 
@@ -329,36 +328,49 @@
 Para implementar as interfaces e construir os *workers* basta editar os *templates* conforme abaixo:
 
 **REGRAS**: Implemente todos os métodos solicitados respeitando os tipos dos parâmetros e de retorno. Não troque os 
 nomes dos parâmetros.
 
 **worker_pub**:
 
-- Abra o arquivo '**pub.py**', que se encontra na pasta '**worker_pub**', e implemente os métodos da interface 
+- Abra o arquivo '**pub1.py**', que se encontra na pasta '**worker_pub/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceCLF** através da classe **ModeloCLF**. Leia os comentários, eles te guiarão na implementação.
+ 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_pub**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
 
 **worker_retrain**:
 
-- Abra o arquivo '**retrain.py**', que se encontra na pasta '**worker_retrain**', e implemente os métodos da interface 
+- Abra o arquivo '**retrain1.py**', que se encontra na pasta '**worker_retrain/models**', e implemente os métodos da interface 
 **ModelPublicationInterfaceRETRAIN** através da classe **ModeloRETRAIN**. Leia os comentários, eles te guiarão na 
 implementação.
 
+
+- Abra o arquivo '**params.conf**', que se encontra na pasta '**worker_retrain**', e informe os parâmetros dos modelos.
+Leia os comentários, eles te guiarão na configuração.
+
+
+**NOTA**: É possível publicar um ou mais modelos utilizando uma mesma **Stack**. Para isso, basta fazer as devidas
+configurações de cada um dos modelos nos arquivos '**params.conf**' constantes nas pastas **worker_pub** e **worker_retrain**.
+
 A lib disponibiliza vários métodos úteis que auxiliarão na implementação das interfaces. 
 Todos os métodos estão documentados via [docstrings](https://peps.python.org/pep-0257/) que, geralmente, são 
 renderizadas pelas IDEs ou editores de código facilitando a leitura da documentação. Veja alguns métodos úteis disponíveis:
 
 - **make_log** - Criação do arquivo para geração de logs.
 - **load_datasets** - Carga de datasets.
 - **load_model** - Carga de modelos salvos.
 - **load_production_params**, **load_production_datasets_names**, **load_production_baseline** - Carga das informações 
 dos modelos publicados, salvas através dos artefatos obrigatórios.
 - **convert_artifact_to_pickle** - Conversão de um artefato para o formato pickle.
 - **convert_artifact_to_object** - Conversão de um artefato que está no formato pickle para o objeto de origem.
 
-Explore a documentação para saber das possibilidades de uso da lib.
+Explore a [documentação](https://prodest.github.io/mllibprodest) para saber das possibilidades de uso da lib.
 
 ### Teste o código produzido!
 O repositório da lib disponibiliza os scripts '**test_pub.py**' e '**test_retrain.py**' para realização de testes para 
 verificar se alguns requisitos solicitados estão sendo atendidos. Também é possível criar testes personalizados através da 
 implementação da função '**test**' que se encontra nos scripts '**mytest_pub.py**' e '**mytest_retrain.py**'. Todos 
 estes scripts estão nas pastas **worker_pub** e **worker_retrain**.
```

### Comparing `mllibprodest-1.5.2/src/mllibprodest.egg-info/SOURCES.txt` & `mllibprodest-1.6.0/src/mllibprodest.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 src/mllibprodest/shared_classes.py
 src/mllibprodest/utils.py
 src/mllibprodest.egg-info/PKG-INFO
 src/mllibprodest.egg-info/SOURCES.txt
 src/mllibprodest.egg-info/dependency_links.txt
 src/mllibprodest.egg-info/requires.txt
 src/mllibprodest.egg-info/top_level.txt
+src/mllibprodest/initiators/__init__.py
+src/mllibprodest/initiators/model_initiator.py
 src/mllibprodest/providers_types/__init__.py
 src/mllibprodest/providers_types/local_provider.py
 src/mllibprodest/providers_types/minio_provider.py
 src/mllibprodest/providers_types/mlflow_provider.py
 src/mllibprodest/validators/__init__.py
 src/mllibprodest/validators/test.py
```

