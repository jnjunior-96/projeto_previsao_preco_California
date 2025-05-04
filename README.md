# Previsão de Preços de Imóveis na Califórnia com Regressão Linea


Origem: https://www.kaggle.com/datasets/camnugent/california-housing-prices/data

## Um pouco mais sobre a base

Os dados provém de um censo do EUA de 1990, onde disponibiliza alguns dados sobre grupos de moradores da região e seus imóveis.

[Clique aqui](referencias/01_dicionario_de_dados.md) para ver o dicionário de dados da base utilizado.

## Etapas

Este projeto tem como objetivo construir e avaliar modelos de regressão para prever o valor médio de imóveis no estado da Califórnia, com base em dados demográficos e geográficos provenientes do censo dos EUA de 1990. Foram aplicadas técnicas de análise exploratória, engenharia de atributos, visualização geográfica e modelagem preditiva.

Para isso algumas etapas forma necessárias:

- 📊 **EDA**: análise exploratória e tratamento inicial dos dados.
- 🌍 **GeoPandas & Folium**: visualizações geográficas dos dados e agrupamento por localização.
- 🔢 **Modelos de Regressão**: aplicação e avaliação de modelos como Regressão Linear, Ridge, Lasso e ElasticNet.
- 📈 **Polynomial Features**: avaliação do impacto da transformação polinomial nas variáveis.
- 🧪 **Regularização**: comparação entre os modelos com técnicas de regularização.
- 🏁 **Modelo Final**: seleção do modelo com melhor desempenho e menor custo computacional (Ridge).

- [EDA](notebooks/01-JN-EDA.ipynb): para tratamento e análise dos dados.
- [GeoPandas e Foium](notebooks/03-JN-geo_parte_01.ipynb): para visualização e manipulação de dados geográficos.
- [Modelos de Regressão](notebooks/04-JN-modelos-parte_01_inicio.ipynb): testando modelos de regressão e preprocessamentos.
- [PolynomialFeatures](notebooks/05-JN-modelos-parte_PolynomialFeatures.ipynb): testando regressão polinomial.
- [Regularização](notebooks/06-JN-modelos-parte_ElasticNet.ipynb): testando e comparando outros modelos e regularizações.
- [Modelo escolhido](notebooks/07-JN-modelos-parte_Ridge.ipynb): modelo com melhor desempenho e menor penalização de processamento.


## Streamlit

Uma versão interativa do projeto foi publicada via Streamlit. Acesse o app clicando abaixo:

👉 [Acesse o App de Previsão de Preços](https://projeto-previsao-preco-california.streamlit.app/)

![App Previsão](relatorios/imagens/App%20Previsao%20Preco%20California.png)

## Organização do projeto

```
├── .gitignore         <- Arquivos e diretórios a serem ignorados pelo Git
├── requirements.txt   <- O arquivo de requisitos para reproduzir o ambiente de análise
├── LICENSE            <- Licença de código aberto se uma for escolhida
├── README.md          <- README principal para desenvolvedores que usam este projeto.
|
├── dados              <- Arquivos de dados para o projeto.
|
├── modelos            <- Modelos treinados e serializados, previsões de modelos ou resumos de modelos
|
├── notebooks          <- Cadernos Jupyter. A convenção de nomenclatura é um número (para ordenação),
│                         as iniciais do criador e uma descrição curta separada por `-`, por exemplo
│                         `01-JN-exploracao-inicial-de-dados`.
│
|   └──src             <- Código-fonte para uso neste projeto.
|      │
|      ├── __init__.py  <- Torna um módulo Python
|      ├── config.py    <- Configurações básicas do projeto
|      └── graficos.py  <- Scripts para criar visualizações exploratórias e orientadas a resultados
|
├── referencias        <- Dicionários de dados, manuais e todos os outros materiais explicativos.
|
├── relatorios         <- Análises geradas em HTML, PDF, LaTeX, etc.
│   └── imagens        <- Gráficos e figuras gerados para serem usados em relatórios
```

## Configuração do ambiente

1. Faça o clone do repositório que será criado a partir deste modelo.

    ```bash
    git clone ENDERECO_DO_REPOSITORIO
    ```

2. Crie um ambiente virtual para o seu projeto utilizando o gerenciador de ambientes de sua preferência.

    a. Caso esteja utilizando o `conda`, exporte as dependências do ambiente para o arquivo `ambiente.yml`:

      ```bash
      conda env export > ambiente.yml
      ```

    b. Caso esteja utilizando outro gerenciador de ambientes, exporte as dependências
    para o arquivo `requirements.txt` ou outro formato de sua preferência. Adicione o
    arquivo ao controle de versão, removendo o arquivo `ambiente.yml`.


## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👤 Autor

Desenvolvido por [José Nivaldo](https://www.linkedin.com/in/jnjunior96)  
Entre em contato: jnjunior96@outlook.com


