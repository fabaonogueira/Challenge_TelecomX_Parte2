# 📊 Análise e Predição de Evasão de Clientes (Churn) - TelecomX

Este projeto faz parte da segunda fase do desafio **TelecomX**, com foco em **Machine Learning aplicado à previsão de churn**.  
O objetivo é transformar dados brutos de clientes em **insights estratégicos** para reduzir a evasão e aumentar a retenção.

---

## 🎯 Objetivo
- Identificar fatores que influenciam a evasão de clientes;
- Construir modelos preditivos que estimem a probabilidade de cancelamento;
- Gerar recomendações de negócio baseadas em evidências.

---

## 🔎 Pipeline do Projeto

### 1️⃣ Exploração dos Dados
- Leitura da base `dados_tratados.csv`;
- Análise inicial para entender estrutura e variáveis.

### 2️⃣ Tratamento de Dados
- Remoção de registros inconsistentes/ausentes;
- Criação da base final balanceada para modelagem.

### 3️⃣ Análise Exploratória
- Distribuição de cancelamentos (**churn vs não churn**);
- Correlação entre variáveis e o alvo (`Cancelou`);
- Visualizações sobre permanência, cobrança mensal e tipo de contrato.

### 4️⃣ Preparação para Modelagem
- One-Hot Encoding para variáveis categóricas;
- Balanceamento das classes com **SMOTE**;
- Split em treino (70%) e teste (30%).

### 5️⃣ Modelagem Preditiva
Modelos testados:
- 🌲 **Random Forest Classifier**
- 👥 **K-Nearest Neighbors (KNN)**

Avaliação:
- *Precision*, *Recall*, *F1-score*;
- Matrizes de confusão.

### 6️⃣ Otimização & Interpretação
- **GridSearchCV** para hiperparâmetros da Random Forest;
- Extração da **importância das variáveis**;
- Destaque para fatores como:
  - `Meses_Permanencia`
  - `Cobranca_Total`
  - `Cobranca_Mensal`
  - `Tipo_Contrato`
  - `Serviços adicionais (Segurança Online, Suporte Técnico)`

---

## 🏆 Resultados
- **Random Forest** obteve melhor performance, especialmente no *recall* para churn.
- Principais insights:
  - Clientes com pouco tempo de permanência têm maior risco de evasão;
  - Contratos mais longos reduzem churn;
  - Fatura digital e internet fibra óptica aparecem associados ao aumento da evasão.

---

## 💡 Recomendações de Negócio
1. Programas de retenção nos **primeiros meses** de contrato;
2. Incentivo a **contratos de 1 ou 2 anos**;
3. Ofertas de **serviços adicionais** (Suporte Técnico, Segurança Online);
4. Monitorar clientes de **fibra óptica** para entender causas de insatisfação;
5. Utilizar o modelo de ML para criar **alertas preditivos de risco**.

---

## 🛠️ Tecnologias
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn)
- **Jupyter Notebook**
- **SMOTE** para balanceamento
- **GridSearchCV** para otimização de modelos

---

## 📂 Estrutura do Repositório
``├── dados_tratados.csv # Base de dados processada``

``├── TelecomX_parte2_BR.ipynb # Notebook principal do projeto``

``├── README.md # Documentação``


---

<!-- Início da seção "Contato" -->
<h2>🌐 Contate-me: </h2>
<div>
  <p>Developed by <b>Fábio Nogueira</b></p>
</div>
<p>
<a href="https://www.linkedin.com/in/faanogueira/" target="_blank"><img style="padding-right: 10px;" src="https://img.icons8.com/?size=100&id=13930&format=png&color=000000" target="_blank" width="80"></a>
<a href="https://github.com/faanogueira" target="_blank"><img style="padding-right: 10px;" src="https://img.icons8.com/?size=100&id=AZOZNnY73haj&format=png&color=000000" target="_blank" width="80"></a>
<a href="https://api.whatsapp.com/send?phone=5571983937557" target="_blank"><img style="padding-right: 10px;" src="https://img.icons8.com/?size=100&id=16713&format=png&color=000000" target="_blank" width="80"></a>
<a href="mailto:faanogueira@gmail.com"><img style="padding-right: 10px;" src="https://img.icons8.com/?size=100&id=P7UIlhbpWzZm&format=png&color=000000" target="_blank" width="80"></a> 
</p>
<!-- Fim da seção "Contato" -->

---

✨ *Este projeto demonstra a aplicação prática de Ciência de Dados para resolver problemas de churn em empresas de telecomunicação, combinando análise exploratória, modelagem preditiva e recomendações estratégicas de negócio.*
