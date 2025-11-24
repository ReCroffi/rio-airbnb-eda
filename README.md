# 🏡 Rio de Janeiro Airbnb – EDA Completo

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** utilizando o dataset de anúncios do Airbnb na cidade do **Rio de Janeiro**, realizando desde o carregamento dos dados até a extração de insights relevantes.

---

## 📌 Objetivos do Projeto

- Explorar o comportamento dos preços no Rio de Janeiro.  
- Avaliar a influência de localização, avaliações e tipo de acomodação.  
- Tratar dados ausentes, inconsistentes e duplicados.  
- Criar visualizações úteis para entendimento do mercado imobiliário de curta duração.  
- Gerar insights que possam compor um portfólio profissional.

---

## ⚙️ Tecnologias Utilizadas

- **Python 3**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Plotly Express** (para o mapa interativo)
- **Jupyter Notebook**

---

## 🧹 Tratamento de Dados

### ✔️ 1. Padronização dos nomes das colunas
- Tudo em minúsculas  
- Espaços substituídos por `_`  
- Remoção de caracteres especiais

### ✔️ 2. Remoção de duplicatas
- Exclusão baseada no campo **id**

### ✔️ 3. Análise e tratamento de valores nulos
- Remoção de colunas com **≥80%** de dados ausentes  
- Remoção de linhas com nulos críticos (`price`, `latitude`, `longitude`, `room_type`)  
- Valores nulos nas colunas de review convertidos para **0**  
- Valores nulos em colunas categóricas substituídos por `"Não informado"`

### ✔️ 4. Ajustes finais
- Conversão de tipos  
- Verificação de consistência  

---

## 📊 Principais Análises Realizadas

### **1. Distribuição de Preços**
- Preços altamente assimétricos  
- Necessidade de limitar eixo X (ex.: 0–1000) para melhor visualização  
- Presença de outliers esperados em imóveis de luxo

---

### **2. Efeito da Localização no Preço**
Insight principal:

> **A localização é determinante — bairros mais caros chegam a ser 42× mais caros que os mais baratos.**

Exemplo:
- Maricá — **R$ 2500**
- Maria da Graça — **R$ 59**

📍 Conclusão:  
Localização explica uma **grande parte da variação no preço** no Rio de Janeiro.

---

### **3. Tipo de Acomodação**
- Apartamentos inteiros possuem preço médio bem maior que quartos privados.  
- Cálculo de diferença percentual incluído no notebook.

---

### **4. Avaliações e Preço**
Insight:

> **Avaliações têm efeito leve a moderado no preço.**

- Correlação baixa (geralmente <0.30)  
- Linha de tendência pouco inclinada  
- A avaliação influencia, mas não é decisiva

---

### **5. Mapa Interativo**
- Construído com `scatter_mapbox`  
- Exibe distribuição espacial dos preços  
- Facilita identificar zonas com forte concentração de imóveis premium

---

## 📝 Principais Insights

- 🌍 **Localização é o fator mais forte** na definição do preço.  
- 🏢 **Apartamentos inteiros** são significativamente mais caros que quartos privados.  
- ⭐ **Avaliações têm influência menor**, indicando que hóspedes priorizam localização e tipo de acomodação.  
- 🗺️ Mapa mostra claramente regiões de preços elevados como Copacabana, Joá e Barra da Tijuca.

---

## 🚀 Próximos Passos

- Aplicar modelos de regressão para prever preços  
- Criar um dashboard no Power BI ou Tableau  
- Explorar sazonalidade se houver dados mensais  
- Analisar disponibilidade e dias mínimos de hospedagem

---

## 📧 Contato

Se quiser ver mais projetos ou falar comigo:

**Renan Croffi**  
GitHub: https://github.com/ReCroffi  
LinkedIn: https://www.linkedin.com/in/renancroffi/

---

### ✔️ Arquivo gerado automaticamente a partir do notebook enviado.

