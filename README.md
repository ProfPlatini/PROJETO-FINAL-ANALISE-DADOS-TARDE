# 🚗 Previsão de Preços de Carros Usados com Machine Learning

> Projeto final desenvolvido durante o curso de **Fundamentos de Inteligência Artificial e Análise de Dados**.

---

## 📋 Sobre o Projeto

Este projeto consiste em uma solução de ponta a ponta (*End-to-End*) de Machine Learning para estimar o valor de mercado de veículos usados. A partir de uma base de dados histórica (`dataset_carros_usados.csv`), o modelo analisa padrões e correlações para realizar previsões de preços via uma **API REST** desenvolvida em Flask, que é consumida por uma interface web interativa.

---

## 🔗 Links do Projeto (Em Produção)

| Plataforma | Link de Acesso | Descrição |
| :--- | :--- | :--- |
| 🌐 **Site / FrontEnd** | [wheel-price-predictor.lovable.app](https://wheel-price-predictor.lovable.app/) | Interface web interativa para realizar previsões de forma intuitiva. |
| 🚀 **API REST / BackEnd** | [projeto-final-analise-dados-tarde.onrender.com](https://projeto-final-analise-dados-tarde.onrender.com) | Servidor na nuvem (Render) hospedando o modelo de Machine Learning. |
| 📦 **Repositório GitHub** | [ProfPlatini/PROJETO-FINAL-ANALISE-DADOS-TARDE](https://github.com/ProfPlatini/PROJETO-FINAL-ANALISE-DADOS-TARDE) | Código-fonte, base de dados e documentação. |

---
<<<<<<< HEAD
### Arquitetura
O modelo de M.L. está hospedado no Render.com, funcionando como uma API, retornando o preço estimado no formato JSON quando realizada uma requisição do tipo *POST* para o link: https://projeto-final-analise-dados-tarde.onrender.com/prever 

**Observação**: Para testes iniciais, realizar uma requisição do tipo GET para o link:
https://projeto-final-analise-dados-tarde.onrender.com

=======

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes ferramentas, bibliotecas e frameworks:

### 🐍 Linguagem & Machine Learning
* **[Python 3](https://www.python.org/)**: Linguagem principal do projeto.
* **[Pandas](https://pandas.pydata.org/) & [NumPy](https://numpy.org/)**: Manipulação, tratamento e análise exploratória de dados.
* **[Scikit-Learn](https://scikit-learn.org/)**: Construção, treinamento e avaliação do modelo de regressão linear/machine learning.
* **[Seaborn](https://seaborn.pydata.org/)**: Visualização de dados e geração de gráficos estatísticos.

### 🌐 BackEnd & API
* **[Flask](https://flask.palletsprojects.com/)**: Framework micro-web utilizado para estruturar os endpoints da API.
* **[Flask-CORS](https://flask-cors.readthedocs.io/)**: Habilitação de requisições de diferentes domínios (*Cross-Origin Resource Sharing*), permitindo a comunicação com o front-end.

### ☁️ Deploy, CD & FrontEnd
* **[Render](https://render.com/)**: Hospedagem em nuvem da API REST com entrega contínua (CD).
* **[Lovable](https://lovable.dev/)**: Desenvolvimento e hospedagem da interface Web (FrontEnd).

>>>>>>> e81d8ba3173ab198eccc4bff0417ef0a2e5b3b03
---

## ⚙️ Variáveis do Modelo

Para estimar o valor de um veículo, o modelo leva em consideração 4 variáveis principais (features):
1. **Ano de fabricação:** Ano do modelo/fabricação do veículo.
2. **Quilometragem:** Distância total percorrida (em km).
3. **Motor:** Potência ou cilindrada do motor (ex: 1.0, 1.6, 2.0).
4. **Quantidade de revisões:** Número de revisões periódicas realizadas no histórico do veículo.

---

## 🚀 How to Use (Como Utilizar)

Você pode testar e utilizar o projeto de três formas diferentes: pela **Interface Web**, consumindo a **API REST** direto no seu código/terminal ou executando o projeto **Localmente**.

### 1️⃣ Opção A: Utilizando a Interface Web (Mais Rápido)
1. Acesse o site oficial: [https://wheel-price-predictor.lovable.app/](https://wheel-price-predictor.lovable.app/).
2. Preencha os campos com os dados do veículo (Ano, Quilometragem, Motor e Revisões).
3. Clique no botão de cálculo para visualizar a estimativa de valor gerada pelo modelo em tempo real.

---

### 2️⃣ Opção B: Consumindo a API REST (Em Nuvem)

#### 🔸 Teste de Status (GET)
Para verificar se a API está online, envie uma requisição do tipo `GET` para a rota principal:
```http
GET [https://projeto-final-analise-dados-tarde.onrender.com/](https://projeto-final-analise-dados-tarde.onrender.com/)
