# 📊 Repositório: miniguia-analise-dados-python

Bem-vindo(a) ao **Miniguia de Estudos de Análise de Dados com Python**! Este repositório foi criado como um projeto de consolidação de conhecimentos, documentando a jornada de aprendizado sobre como transformar dados brutos em decisões estratégicas utilizando a linguagem Python e suas principais bibliotecas.

---

## 🎯 Contexto e Objetivos
O assunto escolhido para este caderno temático é a **Análise de Dados com Python aplicada a Negócios e Finanças**. A análise de dados deixou de ser uma disciplina puramente estatística para se tornar o pilar central das tomadas de decisão estratégicas modernas. O Python consolidou-se como o padrão da indústria devido à sua versatilidade, sintaxe simples e pelo seu poderoso ecossistema de bibliotecas.

**Objetivos de Estudo:**
1. Compreender o ciclo completo de análise de dados (da coleta e limpeza à visualização e modelagem preditiva).
2. Dominar as estruturas e funcionalidades das principais bibliotecas: NumPy, Pandas, Matplotlib, Seaborn e Scikit-Learn.
3. Aplicar esses conhecimentos na resolução de problemas reais de negócios, como previsão de *churn*, análises econômicas e auditoria inteligente.

---

## 📚 Curadoria de Fontes
Para a construção deste material, foram selecionadas e carregadas no NotebookLM as seguintes fontes abertas, focadas tanto em fundamentos práticos quanto acadêmicos:

1. **E-Book: Do Zero à Análise de Dados Econômicos e Financeiros com Python** (Análise Macro) - *Fonte rica em processos metodológicos e ciclo da análise de dados.*
2. **Python para Processamento de Dados** (CEGRAF UFG / Embrapii) - *Apostila detalhada abordando operações multidimensionais com NumPy, Pandas e visualização de dados.*
3. **Uma introdução à análise de dados usando pandas, matplotlib e seaborn** (Casagrande & Silva, UFMT) - *Artigo focado nas etapas estruturadas de coleta, limpeza e Análise Exploratória de Dados (EDA).*
4. **O Uso da Linguagem Python Aplicada à Perícia Financeira** (Revista Gestão e Conhecimento) - *Estudo de caso aplicado mostrando a automação da coleta de indicadores do Banco Central via APIs oficiais.*
5. **Como Usar Python Para Analisar Dados: Passo a Passo** (Blog Tera) - *Guia conceitual voltado para a estruturação mental do analista e a resolução de perguntas de negócios.*

---

## 🧠 Engenharia de Prompts e "Cicatrizes"

Para extrair os melhores *insights* das fontes no NotebookLM, a seguinte engenharia de prompts foi aplicada:

*   **Prompt 1:** *"Como o Python é aplicado em casos reais de negócios?"*
    *   **Resultado e Referência:** A IA gerou exemplos excelentes de aplicações no E-commerce, análise de *Churn* (ex: Netflix), RH, e integrações via APIs financeiras.
    *   **Cicatriz (Troubleshooting):** Inicialmente, a IA retornava apenas que Python servia para criar gráficos e treinar máquinas, de forma muito teórica. O prompt foi refinado exigindo exemplos de *negócios reais* contidos nos textos, fazendo com que ela trouxesse a aplicação do modelo de classificação para risco de evasão (Churn) e cálculos de desempenho financeiro.
*   **Prompt 2:** *"Liste as etapas do Ciclo de Análise de Dados e descreva as principais bibliotecas Python usadas em cada etapa."*
    *   **Resultado e Referência:** A resposta segmentou de forma didática as fases: Objetivo, Dados (coleta com `requests`, `python-bcb`), Exploração (EDA com `Pandas`), Modelagem (`Scikit-learn`) e Visualização (`Matplotlib`, `Seaborn`).
    *   **Cicatriz (Troubleshooting):** No primeiro teste, a ferramenta apenas listou o que as bibliotecas faziam (ex: "Pandas serve para tabelas"). Tivemos que guiar a IA explicitamente a cruzar o "Ciclo de Vida do Dado" (presente na fonte da Análise Macro) com a "Apresentação de Bibliotecas", para conectar o *framework* mental ao código.

---

## 🚀 Miniguia de Estudo 

### 📌 Resumo

#### 1. O Ciclo de Análise de Dados
O processo de resolver problemas com dados não é linear, sendo composto por fases iterativas:
*   **Objetivo:** Definição clara do problema de negócio (ex: queda de engajamento de usuários na Netflix).
*   **Coleta de Dados:** Extração e identificação de informações em bancos SQL, planilhas Excel ou APIs Web.
*   **Exploração (EDA) e Limpeza:** Tratamento de dados faltantes (NaN), remoção de duplicatas, e identificação de anomalias (outliers).
*   **Modelagem:** Aplicação de análises estatísticas, econometria ou *Machine Learning* para classificar, prever ou gerar inferências.
*   **Validação:** Verificação da acurácia e avaliação dos resultados usando métricas e validação cruzada.
*   **Implantação:** Tomada de decisão, comunicação via relatórios, *dashboards* ou integração do modelo preditivo aos sistemas da empresa.

#### 2. O Ecossistema de Bibliotecas Python
*   **NumPy:** Base matemática do Python. Cria arrays multidimensionais (vetores e matrizes) altamente eficientes. Permite vetorização matemática, eliminando estruturas lentas de repetição de código (loops).
*   **Pandas:** Usado para manipulação e alinhamento de dados tabulares e relacionais através de suas estruturas bidimensionais (`DataFrames`) e unidimensionais (`Series`). Essencial na higienização de dados e leitura de arquivos variados (CSV, JSON, Excel).
*   **Matplotlib e Seaborn:** As principais aliadas na visualização. A Matplotlib gera gráficos linha, histogramas e permite combinar múltiplos gráficos de forma customizada. Já a Seaborn foca na interface visual de alto nível e estética de dados estatísticos (ex: *pair plots*, *boxplots* e matrizes de correlação).
*   **Scikit-Learn:** O padrão industrial para o desenvolvimento de modelos preditivos e aprendizado de máquina (Machine Learning), com sintaxe unificada de ajustes (`.fit()`) e previsões (`.predict()`).

### 📖 Glossário de Conceitos
*   **Array / ndarray:** Estrutura fundamental do *NumPy* que armazena dados de forma contígua na memória do computador, permitindo computação científica rápida e de alto desempenho.
*   **Broadcasting:** Recurso poderoso do *NumPy* para realizar operações matemáticas automatizadas entre matrizes/arrays de formas e tamanhos diferentes, ajustando as dimensões de forma inteligente.
*   **DataFrame:** Estrutura do *Pandas* em formato tabular e bidimensional (composta por linhas e colunas), bastante comparável a uma planilha do Excel ou a uma tabela de banco de dados SQL.
*   **EDA (Análise Exploratória de Dados):** Etapa focada em utilizar descrições estatísticas e visualizações gráficas para descobrir padrões ocultos e investigar relacionamentos entre variáveis antes da construção de qualquer modelo analítico complexo.
*   **Outliers:** Elementos ou valores que se desviam e diferem anormalmente da maioria das outras observações em um conjunto de dados. Eles podem mascarar estatísticas reais (como a média aritmética) e afetar severamente as previsões.
*   **Series:** Estrutura base de dados unidimensional (coluna individual) do *Pandas* capaz de armazenar qualquer tipo de dado, com índices flexíveis.

### 💡 Prompts Reutilizáveis para Revisão
Para futuras revisões no NotebookLM ou em outros *LLMs* usando bases de dados e arquivos de estudo, aplique estes prompts:

1. **Para dominar novos métodos e comandos do Python:**
   > *"Estou aprendendo o método `[NOME DO MÉTODO, ex: pandas.merge()]`. Explique de forma prática para que ele serve, de acordo com o material fonte, e forneça 2 exemplos simples de código comparando com `[OUTRO MÉTODO, ex: pandas.join()]`."*
2. **Para entender fluxo de negócios:**
   > *"No contexto de `[ÁREA, ex: Varejo / Mercado Financeiro]`, descreva passo a passo como realizar a `[TAREFA, ex: Análise Exploratória de Dados]` baseando-se no ciclo de análise detalhado nos documentos."*
3. **Para simular desafios técnicos (Troubleshooting):**
   > *"Estou lidando com uma base de dados que possui muitos valores nulos (NaN) na coluna de idade e letras maiúsculas/minúsculas misturadas na coluna de nomes. Crie um pequeno roteiro em tópicos sobre como eu deveria higienizar esses dados utilizando o Pandas, justificando o porquê de cada técnica."*
