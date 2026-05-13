# wine-quality-classification
Classificação de qualidade de vinhos com Machine Learning — POSTECH Fase 2
# 🍷 Wine Quality Classification — ML

Modelo de Machine Learning para prever a qualidade de vinhos com base em
características físico-químicas. Projeto da Fase 2 do curso DTAT — POSTECH.

## 🎯 Objetivo
Classificar vinhos como **Alta Qualidade** (nota ≥ 7) ou **Baixa/Média Qualidade**
(nota < 7) usando dados físico-químicos, substituindo parte da avaliação humana.

## 📁 Estrutura
├── notebooks/analise_vinho.ipynb   # Pipeline completo de análise e ML
├── results/                        # Gráficos gerados
│   ├── eda_vinho.png
│   ├── correlacao_vinho.png
│   ├── modelos_vinho.png
│   └── roc_vinho.png
└── README.md

## 📊 Dataset
- Fonte: [Wine Quality Dataset — Kaggle](https://www.kaggle.com/datasets/yasserh/wine-quality-dataset)
- 1.143 amostras de vinho tinto
- 11 variáveis físico-químicas

## 🤖 Modelos e Resultados

| Modelo | Acurácia | AUC |
|---|---|---|
| Regressão Logística | 86% | 0,842 |
| **Random Forest** ✅ | **92%** | **0,909** |

## 🏆 Principais Descobertas
1. **Teor alcoólico** é o fator mais importante — vinhos de alta qualidade
   têm ~12% de álcool vs ~10% dos demais
2. **Sulfatos** elevados estão associados à alta qualidade
3. **Acidez volátil** baixa é característica dos melhores vinhos

## 🎯 Recomendações
- Monitorar teor alcoólico como indicador principal durante produção
- Controlar acidez volátil na fermentação
- Usar o modelo para triagem antes da avaliação humana
- Potencial de redução de custo nas avaliações manuais

## 🛠️ Tecnologias
Python · Pandas · Scikit-learn · Matplotlib · Seaborn · Google Colab
