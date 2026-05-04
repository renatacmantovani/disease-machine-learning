# 🧠 Machine Learning aplicada ao diagnóstico de Transtornos Mentais

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-green)](https://scikit-learn.org/)

Modelo de Machine Learning aplicada ao Diagnóstico de Transtornos Mentais partindo de sintomas para classificação de **Transtorno do Pânico**, **Ansiedade** e **Esquizofrenia** utilizando análise comparativa entre Árvore de Decisão e
Random Forest. O **Random Forest** apresentou desempenho superior com alta capacidade de generalização (97%).

## 📊 Visão Geral

Este projeto implementa e compara dois algoritmos de aprendizado de máquina para auxiliar no diagnóstico diferencial de transtornos mentais com base em sintomas relatados.

### 🎯 Objetivos
- Classificar corretamente três condições psiquiátricas
- Comparar o desempenho entre Árvore de Decisão e Random Forest
- Identificar os sintomas mais relevantes para cada diagnóstico

## 📂 Estrutura do Repositório

- **data/** - Pasta com os dados
  - `dataset_cortado.csv` - Base filtrada (2.997 amostras, 21 sintomas)

- **jupyter/** - Notebooks Jupyter
  - `Disease-ML.ipynb` - Análise completa do projeto

- **report/** - Artigos e documentação
  - `Disease Report - Machine Learning.pdf` - Artigo com análises detalhadas

- **Arquivos raiz**
  - `requirements.txt` - Dependências do projeto
  - `README.md` - Documentação principal

## 🗃️ Base de Dados

- **Fonte original**: [Diseases and Symptoms Dataset](https://www.kaggle.com/datasets/dhivyeshrk/diseases-and-symptoms-dataset/code) (Kaggle)
- **Condições selecionadas**: 
  - Transtorno do Pânico
  - Ansiedade
  - Esquizofrenia
- **Amostras**: 2.997 registros
- **Sintomas relevantes**: 21 (após limpeza e seleção)

## 🔧 Como Reproduzir

### Pré-requisitos
- Python 3.8+
- Jupyter Notebook
- Git LFS (para baixar o dataset)

### Passos

1. **Clone o repositório**
```bash
git clone https://github.com/renatacmantovani/disease-machine-learning.git
cd disease-machine-learning
```
2. **Instale as dependências**

```bash
pip install -r requirements.txt
```
3. **Execute o notebook**

```bash
jupyter notebook Disease-ML.ipynb
```
4. **Ou rode em modo headless**

```bash
jupyter nbconvert --to notebook --execute Disease-ML.ipynb
```

## 📦 Dependências
```text
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
```

## 🛠️ Metodologia

### Pré-processamento:

- Seleção de 3 classes específicas
- Limpeza e padronização dos sintomas
- Redução dimensional baseada em relevância clínica

### Divisão dos Dados
- Treino: 80%
- Validação: 10%
- Teste: 10%

- **Validação cruzada: 5-folds** 

## Algoritmos Implementados
- 🌳 Árvore de Decisão (baseline)
- 🌲 Random Forest (melhor performance)


## 📄 Licença
Este projeto está sob licença MIT - veja o arquivo LICENSE para detalhes.

## 🙏 Agradecimentos
- Kaggle pelo dataset Diseases and Symptoms Dataset
- Comunidade de ciência de dados por frameworks e ferramentas open-source


