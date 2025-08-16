# 📊 Telecom X – Parte 2: Prevendo Churn  

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Contribuições](https://img.shields.io/badge/contribui%C3%A7%C3%B5es-bem--vindas-brightgreen)

---

## 📖 Introdução  
A evasão de clientes (*Churn*) é um dos maiores desafios para empresas de telecomunicações.  
Identificar com antecedência quais clientes têm maior probabilidade de cancelar seus serviços permite a adoção de estratégias de retenção mais eficazes, reduzindo custos e aumentando a satisfação.  

Neste projeto, damos continuidade à análise exploratória realizada na **Parte 1** e avançamos para a **construção de modelos preditivos de Machine Learning**.  

---

## 🎯 Objetivos  
- Preparar os dados para modelagem (tratamento, encoding e normalização).  
- Analisar correlação e selecionar as variáveis mais relevantes.  
- Treinar e avaliar **dois ou mais modelos de classificação**.  
- Comparar o desempenho com métricas adequadas.  
- Interpretar os resultados, incluindo a **importância das variáveis**.  
- Apontar conclusões estratégicas para reduzir a evasão de clientes.  

---

## 🧰 Tecnologias Utilizadas  
- **Python 3.10+**  
- **Pandas** e **NumPy** → manipulação e análise de dados  
- **Matplotlib** e **Seaborn** → visualizações  
- **Scikit-learn** → pré-processamento, modelagem e métricas  
- **XGBoost / Random Forest** → modelos mais robustos de classificação  

---

## 🔎 Etapas do Projeto  

### 1. Preparação dos Dados  
- Importação da base tratada (limpeza já realizada na Parte 1).  
- Encoding de variáveis categóricas.  
- Normalização de variáveis numéricas.  

### 2. Seleção de Variáveis  
- Análise de correlação entre variáveis numéricas.  
- Aplicação de técnicas de seleção de features.  

### 3. Modelagem  
Modelos testados:  
- **Regressão Logística** (baseline, modelo simples e interpretável).  
- **Random Forest / XGBoost** (modelos mais robustos e não-lineares).  

### 4. Avaliação  
Métricas utilizadas:  
- Accuracy  
- Precision  
- Recall (foco principal, pois churn é mais sensível a falsos negativos)  
- F1-score  
- ROC-AUC  

Além disso:  
- Matrizes de confusão  
- Curva ROC  

### 5. Interpretação dos Resultados  
- Importância das variáveis nos modelos.  
- Identificação dos fatores que mais influenciam a evasão.  

---

## 📈 Resultados e Conclusões  
- O modelo **XGBoost/Random Forest** apresentou melhor desempenho em termos de **Recall e AUC**, se mostrando mais adequado para prever clientes em risco de churn.  
- Principais fatores que influenciam a evasão:  
  - Tipo de contrato (mensal tende a ter mais churn).  
  - Tempo de permanência (clientes novos apresentam maior evasão).  
  - Valor mensal da fatura (valores mais altos correlacionam com maior cancelamento).  
- Estratégias sugeridas:  
  - Oferecer planos de fidelização e descontos para clientes de maior risco.  
  - Criar programas de retenção específicos para novos clientes.  
  - Monitorar clientes com alto ticket médio mensal e oferecer alternativas mais acessíveis.  

---

## 🚀 Como Utilizar  

### 🔧 Requisitos  
Certifique-se de ter instalado:  
- Python 3.10+  
- Git  
- Pip  

### 📥 Clonar o Repositório  
```bash
git clone https://github.com/SEU_USUARIO/telecom-churn.git
cd telecom-churn
