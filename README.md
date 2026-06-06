# Sistema de Apoio à Tomada de Decisão - Campanhas PRF 2025

Este repositório contém a implementação de um modelo preditivo baseado em **Árvore de Decisão** para analisar a gravidade de sinistros de trânsito ocorridos nas rodovias federais brasileiras durante o ano de 2025. O objetivo principal é dar suporte à tomada de decisão estratégica para o planejamento e direcionamento de verbas em campanhas educativas de trânsito.

O projeto foi desenvolvido como parte da avaliação **AV1** da disciplina de **Sistemas de Apoio à Tomada de Decisão** do curso de **Sistemas de Informação**.

## Tecnologias e Ferramentas Utilizadas

* **Linguagem de Programação:** Python 3.x
* **Ambiente de Execução Recomendado:** VS Code, Jupyter Notebook ou Google Colab
* **Principais Bibliotecas:**
    * `pandas` (Manipulação e tratamento de dados)
    * `numpy` (Operações matemáticas)
    * `scikit-learn` (Algoritmo de Machine Learning e métricas)
    * `matplotlib` (Visualização gráfica da árvore)

## Estrutura do Repositório

````
├── datatran2025.csv      # Base de dados bruta da PRF
├── ArvoreDecisao.ipynb   # Script Python com a solução estruturada
└── README.md             # Documentação do projeto
````

Como Executar o Projeto na Sua Máquina
Siga o passo a passo abaixo para configurar o ambiente e rodar o código localmente.

# 1. Clonar o Repositório
Abra o terminal do seu computador e mude para o diretório onde deseja salvar o projeto. Em seguida, execute:
````
git clone https://github.com/JotaV232323/arvore-de-decisao.git
cd arvore-de-decisao
````
# 2. Baixar a Base de Dados
Acesse o Portal de Dados Abertos do Governo Federal.

Faça o download do conjunto de dados de Sinistros de Trânsito Agrupados por Ocorrência referente ao ano de 2025.

Extraia e mova o arquivo .csv para a raiz deste projeto (mesma pasta onde está o arquivo).

Garanta que o arquivo esteja nomeado exatamente como datatran2025.csv.

# 3. Instalar as Dependências
Instale as bibliotecas necessárias rodando o seguinte comando no terminal:
````
pip install scikit-learn pandas numpy matplotlib
````
# 4. Executar o Script Python
Com o ambiente configurado e a base de dados na pasta correta, execute o script:
````
python modelo_transito.py
````
# Metodologia e Resultados Obtidos
Algoritmo: Árvore de Decisão (DecisionTreeClassifier) configurada com o critério de Entropia para o cálculo do Ganho de Informação.

Divisão de Dados: 70% da base foi utilizada para Treino e 30% para Teste, utilizando o random_state=42 para garantir a reprodutibilidade exata dos resultados.

Desempenho Geral: O modelo alcançou uma Acurácia de 87,01% e um Recall de 100% para a classe de acidentes com vítimas, demonstrando excelente sensibilidade e segurança para aplicação em políticas públicas.

Os atributos identificados como mais relevantes pelo modelo para a classificação de gravidade foram:

Incêndio em Veículos (66,98% de importância)

Ingestão de Álcool pelo Condutor (18,87% de importância)

Atropelamento de Pedestres (6,05% de importância)

# Contato
Autor: João Vitor Barbosa Mendes
Curso: Sistemas de Informação
