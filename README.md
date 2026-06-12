# Trabalho Análise C3

> Neste trabalho, será desenvolvido todo o código referente às atividades solicitadas na avaliação C3 da disciplina de **Análise de Dados**.

### Tópicos Abordados
O notebook foi estruturado para cobrir as seguintes etapas do pipeline de dados:

* **Análise Exploratória de Dados (EDA):** Compreensão da distribuição e correlação das variáveis.
* **Feature Engineering:** Tratamento e criação de novas variáveis para otimização dos modelos.
* **Aprendizagem Supervisionada:** Treinamento de um dos modelos de Aprendizagem Supervisionada selecionado.
* **Aprendizagem Não Supervisionada:** Treinamento de um dos modelos de Aprendizagem Não Supervisionada selecionado.
* **Métricas de Avaliação:** Avaliar o desempenho dos modelos de aprendizagem supervisionada, comparando-os entre si e com o modelo não supervisionado escolhido.

### Base de Dados
Para a execução deste projeto, utilizamos o dataset oficial proposto pela atividade:

[Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-pricesadvanced-regression-techniques/data)

### Como Rodar o Projeto

Este projeto utiliza o **`uv`** para gerenciar as dependências e o ambiente virtual Python.

### Passo a Passo

1. **Instalar as dependências e criar o ambiente virtual:**
   No diretório do projeto, execute:
   ```bash
   uv sync
   ```
2. **Executar o Jupyter Notebook:**
   Você pode rodar o notebook de duas formas:

     Execute o comando abaixo para abrir a interface web do Jupyter diretamente no seu navegador:
     ```bash
     uv run --with jupyter jupyter notebook notebook.ipynb
     ```
