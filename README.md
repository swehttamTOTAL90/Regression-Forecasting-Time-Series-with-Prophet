# Previsão de Séries Temporais com Prophet

Aplicação em **Python** para previsão de níveis de ozônio (**O₃**) utilizando a biblioteca **Prophet**, com interface interativa desenvolvida em **Streamlit**.

O usuário informa o horizonte de previsão em dias e a aplicação gera estimativas futuras, um gráfico interativo e uma tabela com os valores previstos.

## Funcionalidades

- Carregamento de um modelo Prophet previamente treinado.
- Previsão de níveis futuros de O₃.
- Seleção do horizonte de previsão pelo usuário.
- Visualização interativa com Plotly.
- Exibição das previsões em formato de tabela.
- Exportação dos resultados em CSV.

## Desempenho do modelo

O modelo foi treinado com dados até **05/05/2023** e, conforme registrado na aplicação, apresentou **RMSE de 17,43** nos dados de teste.

## Tecnologias

- Python
- Prophet
- Pandas
- Streamlit
- Plotly

## Estrutura do projeto

```text
Regression-Forecasting-Time-Series-with-Prophet/
├── App.py
├── modelo_TEMP_prophet.json
├── requirements.txt
└── README.md
```

## Como executar

1. Clone o repositório.
2. Crie e ative um ambiente virtual.
3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute a aplicação:

```bash
streamlit run App.py
```

## Como funciona

O arquivo `App.py` carrega o modelo Prophet serializado em `modelo_TEMP_prophet.json`. Quando o usuário informa a quantidade de dias e solicita a previsão, a aplicação cria o período futuro, executa o modelo e apresenta os resultados em um gráfico e em uma tabela.

## Objetivo do projeto

O projeto foi desenvolvido para aplicar conceitos de **séries temporais**, avaliação de modelos e criação de aplicações interativas para disponibilização de previsões.

---

Projeto desenvolvido para fins de estudo e portfólio em **Data Science** e **Machine Learning**.