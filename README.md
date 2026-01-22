# 💧 EY AI & Data Challenge 2026: Water Quality Prediction

Este repositório contém a solução desenvolvida para o desafio global da Ernst & Young (EY), focado na previsão da qualidade da água em corpos hídricos superficiais na África do Sul, utilizando Inteligência Artificial e Dados Geoespaciais.

## 🎯 Objetivo do Desafio
[cite_start]O objetivo principal é desenvolver modelos robustos de Machine Learning capazes de prever a qualidade da água em locais não vistos durante o treinamento (generalização espacial)[cite: 28, 35].

[cite_start]Os modelos devem prever três parâmetros críticos[cite: 30]:
1.  **Alcalinidade Total (Total Alkalinity):** Relacionada à geologia e capacidade de neutralizar ácidos.
2.  **Condutividade Elétrica (Electrical Conductance - EC):** Indicador de salinidade e poluição dissolvida.
3.  **Fósforo Reativo Dissolvido (Dissolved Reactive Phosphorus - DRP):** Indicador de eutrofização (fertilizantes/esgoto).

[cite_start]A métrica de avaliação é o **R² (Coeficiente de Determinação)** médio entre as três variáveis[cite: 230].

## 🛰️ Dados e Fontes
O projeto utiliza uma abordagem multimodal, combinando dados tabulares de estações de coleta com sensoriamento remoto:

* [cite_start]**Dados de Treino (Ground Truth):** Coletas realizadas entre 2011 e 2015 em ~200 locais na África do Sul[cite: 31].
* [cite_start]**Imagens de Satélite:** Landsat Level-2 (Bandas espectrais e índices como NDVI/NDWI) para monitorar uso do solo e características da água[cite: 150].
* [cite_start]**Dados Climáticos:** TerraClimate (Precipitação, Temperatura, Evapotranspiração) para capturar sazonalidade e escoamento superficial[cite: 176].

## 🛠️ Tech Stack & Infraestrutura
[cite_start]O projeto foi desenvolvido majoritariamente no ambiente **Snowflake AI Data Cloud**, conforme recomendação do desafio[cite: 213].

* **Linguagem:** Python 3.8+
* **Plataforma:** Snowflake (Data Engineering & Model Training)
* **Bibliotecas Principais:** `pandas`, `scikit-learn`, `xgboost`, `rasterio`, `geopandas`, `snowpark`.

