# 📊 Telecom X – Parte 2: Prevendo Churn  

![Python](https://img.shields.io/badge/python-3.11-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.3.1-orange?logo=scikit-learn)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Viz-009688)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Charts-11557c)

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

- Python 3.11  
- Pandas, NumPy (manipulação de dados)  
- Scikit-Learn (modelos de Machine Learning)  
- Seaborn, Matplotlib (visualização de dados)  

---

## 🔬 Análise e Modelagem

### 1. Pré-processamento

- Tratamento de valores nulos e inconsistentes  
- Codificação de variáveis categóricas (One-Hot Encoding)  
- Normalização de variáveis numéricas  

### 2. Análise Exploratória

- Distribuição da variável target `evasao`  
- Correlação entre variáveis numéricas  
- Identificação das principais variáveis relacionadas ao churn  

### 3. Modelos Preditivos

Foram treinados dois modelos principais:

1. **Regressão Logística**  
   - Interpretável, captura bem clientes de alto risco (recall = 0.79)  
   - Destaques: `total_gasto`, `total_servico_mes`, `meses_contrato`

2. **Random Forest**  
   - Captura relações não-lineares e interações complexas  
   - Destaques: `total_gasto`, `meses_contrato`, `total_servico_mes`  

---

## 📊 Resultados

- Regressão Logística:  
  - Accuracy: 74%  
  - Recall churn: 79%  
  - F1-score churn: 62%  

- Random Forest:  
  - Accuracy: 79%  
  - Recall churn: 48%  
  - F1-score churn: 55%  

**Insight Estratégico:**  
- Para estratégias de retenção, a **Regressão Logística** é mais eficaz na identificação de clientes de risco.  
- Random Forest complementa ao capturar padrões complexos, mas perde recall da classe minoritária.

---

## 💡 Estratégias de Retenção Sugeridas

1. Programas de fidelidade e descontos para clientes de alto gasto  
2. Monitoramento e contato proativo para clientes recém-contratados  
3. Pacotes customizados baseados em perfil de uso  
4. Campanhas de satisfação e suporte personalizado  
5. Alerta para clientes de alto gasto sem engajamento  

---

## 📥 Como Utilizar

1. Clone o repositório:  
```bash
git clone https://github.com/EricPettersonL/Telecom_X_pt2.git
```
2. Abra no Google Colab ou Jupyter Notebook.

3. Instale as dependências (se necessário):
```bash
pip install pandas numpy matplotlib seaborn
```

4. Execute o notebook para reproduzir as análises.
## 📖 Referências

- [Scikit-Learn Documentation](https://scikit-learn.org/stable/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Seaborn Documentation](https://seaborn.pydata.org/)


## ⚡ Autor

Eric Petterson Lima
