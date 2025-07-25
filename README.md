# Classificação Automática de Notícias com NLP: Identificação de Fake News

## Visão Geral do Projeto

Este projeto utiliza técnicas de Processamento de Linguagem Natural (NLP) para desenvolver um modelo de classificação capaz de identificar se uma notícia é **real** ou **falsa** (Fake News) com base **exclusivamente em seu conteúdo textual**. O objetivo principal é auxiliar no combate à desinformação digital, automatizando a identificação de notícias falsas e contribuindo para um ambiente informacional mais confiável.

## Conjunto de Dados

O dataset utilizado para este projeto é o **"Fake and Real News Dataset"**, disponível no Kaggle.

* **Link:** [https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
* **Origem:** Kaggle
* **Tamanho:** Aproximadamente 44.000 notícias, divididas entre as classes "real" e "fake".

**Descrição do Dataset:**
Este conjunto de dados contém manchetes e conteúdos de notícias classificadas como:
* **Reais:** Provenientes de fontes confiáveis como Reuters e HuffPost.
* **Falsas:** Extraídas de sites conhecidos por disseminar desinformação.

Cada entrada no dataset possui os seguintes campos:
* `title`: O título da notícia.
* `text`: O conteúdo completo da notícia.
* `label`: A categoria da notícia (`fake` ou `real`).

## Estrutura do Projeto

O projeto é implementado em um notebook Jupyter (`NLP_FakeNews .ipynb`) e segue as seguintes etapas:

1.  **Preparação do Ambiente e Carregamento dos Dados**
2.  **Pré-processamento de Texto**
3.  **Divisão dos Dados e Vetorização TF-IDF**
4.  **Construção e Treinamento do Modelo (com Early Stopping)**
5.  **Avaliação do Modelo**

## Tecnologias Utilizadas

* **Python**
* **pandas**
* **NumPy**
* **NLTK (Natural Language Toolkit)**
* **scikit-learn**
* **TensorFlow / Keras**
* **Matplotlib / Seaborn**

## Resultados e Conclusão

Este projeto demonstrou um pipeline completo e eficaz para a classificação de notícias falsas usando NLP. O modelo de rede neural, combinado com o pré-processamento de texto e a vetorização TF-IDF, mostrou-se capaz de identificar padrões no conteúdo textual que distinguem notícias reais de falsas. A aplicação do `EarlyStopping` foi fundamental para garantir que o modelo não sofresse *overfitting*, resultando em uma boa capacidade de generalização para dados não vistos.

As métricas de avaliação (acurácia, precisão, *recall*, F1-score) e a matriz de confusão fornecem uma análise detalhada do desempenho do modelo, que se mostra promissor para auxiliar no combate à desinformação digital, automatizando a verificação de conteúdo.
