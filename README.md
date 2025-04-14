# 🧠 Breast Cancer Neural Networks

Este repositório contém o desenvolvimento do **Trabalho Prático 01 da disciplina de Redes Neurais Artificiais (UERJ)**, com foco na **detecção de câncer de mama** utilizando **redes neurais artificiais** desenvolvidas do zero.

## 🎯 Objetivo

Construir e avaliar modelos de redes neurais com diferentes arquiteturas e funções de ativação, a fim de classificar tumores como **malignos ou benignos** com o maior desempenho possível, dentro de uma **divisão de 80% para treino e 20% para teste**.

## 📊 Dataset

- Fonte: [Kaggle - Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- Características:
  - 30 variáveis numéricas extraídas de exames de imagem
  - Alvo: `diagnosis` (M = Maligno, B = Benigno)

## 🧪 Metodologia

- Pré-processamento:
  - Conversão de rótulos para binários (0 e 1)
  - Normalização com `StandardScaler`
- Arquiteturas testadas:
  - 1 camada oculta com 4 neurônios
  - 2 camadas ocultas com 8 neurônios cada
  - 3 camadas ocultas com 6 neurônios cada
- Funções de ativação utilizadas:
  - `linear`
  - `sigmoid`
  - `tanh`
  - `relu`
- Critérios de avaliação:
  - Acurácia no conjunto de teste
  - Perda (`loss`) de treino e validação
  - Análise de subajuste e sobreajuste
- Visualizações:
  - Curvas de perda por época
  - Tabela comparativa de desempenho
  - Matriz de confusão (opcional)
  - Gráficos de comparação entre arquiteturas

## 📈 Resultados

A arquitetura com **3 camadas ocultas de 6 neurônios e função de ativação `tanh`** apresentou o melhor desempenho geral, com **acurácia superior a 85%**, baixa perda de validação e excelente generalização.  
Outras arquiteturas sofreram de **subajuste** (redes muito simples) ou **sobreajuste** (caso de `relu` em redes profundas com alto gap entre treino e teste).

## 📁 Estrutura do Repositório
├── data/ # Dataset original (.csv)
├── notebooks/ # Jupyter Notebooks com os testes 
├── results/ # Gráficos e tabelas salvas 
├── src/ # Código principal (modelos, funções utilitárias) 
└── README.md # Esta documentação

## 📅 Apresentação

- **Data:** 24/04/2025
- **Disciplina:** Redes Neurais Artificiais – UERJ
- **Professor:** Prof. Dr. Fernando R. T. Ferreira

## 👨‍💻 Desenvolvido por

> João Vinicius Carvalho Lamarca Vitral (202010358111)
> Marcelo Bracet (202010357611)  
> Alunos do Instituto Politécnico da UERJ

---

