## Global Solution - Modelagem Linear para Aprendizagem de Máquina

##  Informações do Projeto e Autoria
* **Curso:** Bacharelado em Ciência da Computação (FIAP)
* **Turma:** 1CCPJ
* **Desafio:** Análise Estatística Aplicada à Nova Economia Espacial

###  Integrantes do Grupo
* **[Maria Eduarda Rocha Benjamim]** - RM: `[570554]`
* **[Pedro Henrique Neves]** - RM: `[571382]`
* **[Akin Alexandre Mendes Martins]** - RM: `[572773]`

---

##  01) Seleção e Justificativa da Base de Dados

###  Origem do Dataset
* **Nome Original:** All Space Missions from 1957
* **Arquivo Utilizado:** `Space_Corrected.csv`
* **Fonte:** [Kaggle - Space Missions Dataset](https://kaggle.com)

###  Justificativa Técnica
A transição dos monopólios estatais para a **Nova Economia Espacial** exige decisões corporativas baseadas em alta previsibilidade orçamentária e sustentabilidade operacional. Esta base reúne dados reais de transações aeroespaciais globais desde o início da exploração orbital. 

A escolha do arquivo `Space_Corrected.csv` justifica-se pelo seu potencial analítico rigoroso. Ele apresenta variáveis categóricas para governança operacional (`Company Name`, `Status Mission`) associadas a dimensões métricas financeiras (` Rocket`). O tratamento dos dados permitiu isolar o vetor cronológico (`Datum`) para anos inteiros e limpar strings financeiras complexas, viabilizando uma análise exploratória robusta e fiel ao mercado global real.

---

##  Estrutura Arquitetural do Repositório

```text
├── README.md               # Documentação técnica e guia do projeto (este arquivo)
├── Space_Corrected.csv     # Base de dados real extraída do Kaggle
├── global_solution.ipynb   # Código-fonte Python executável com análises e gráficos
└── relatorio_final.pdf     # Relatório estatístico final formatado para o cliente
```

---

##  Arquitetura de Software e Metodologia Científica

O ecossistema computacional foi construído inteiramente em **Python 3** utilizando o ambiente do **Google Colab**. O script foi projetado sob os seguintes pilares de engenharia de dados:

1. **Tratamento e Engenharia de Atributos:** Limpeza de strings monetárias, remoção de caracteres e conversão do vetor de custos para ponto flutuante (`float`). Extração e conversão de séries temporais para anos discretos (`int`).
2. **Plano de Amostragem Estruturada:** Extração de uma amostra probabilística aleatória e estrita de **100 elementos** para neutralizar vieses temporais, isolando os dados em `variavel_discreta` e `variavel_continua` conforme metodologia proprietária do grupo.
3. **Modelagem de Frequências (TDF):** Construção automatizada de tabelas de distribuição contínua e discreta, mensurando frequências absolutas (`fi`), acumuladas (`fi_acumulada`) e relativas percentuais (`fr%`).
4. **Visualização Avançada com Seaborn:** Geração de gráficos estatísticos integrando o ecossistema Seaborn e Matplotlib, aplicando temas corporativos (`whitegrid`), eixos nomeados e curvas de densidade Kernel (KDE).
5. **Diagnóstico Univariado:** Processamento exato das medidas de tendência central, dispersão e separatrizes (quartis) sobre o vetor de custos.

---

##  Resumo Executivo de Insights Estatísticos

* **Eficiência Orçamentária:** Mais de 50% dos lançamentos comerciais recentes se concentram na faixa inicial de custos (sub-100M). Isso comprova que a reutilização de componentes aeroespaciais reduziu drasticamente as barreiras econômicas de entrada para empresas privadas.
* **Assimetria Positiva:** A média de custo substancialmente maior que a mediana aponta para um mercado assimétrico à direita, puxado por raros megaprojetos governamentais em meio a uma massa de lançamentos de microssatélites ágeis de baixo orçamento.
* **Zona de Previsibilidade:** O mapeamento dos quartis indica que 75% de todo o mercado opera abaixo de USD 130 milhões, delimitando o teto orçamentário ideal para novos fundos de Venture Capital.

---

##  Como Executar o Projeto

1. Faça o clone deste repositório para sua máquina local ou baixe os arquivos.
2. Acesse o [Google Colab](https://google.com).
3. Faça o upload do arquivo `global_solution.ipynb`.
4. No menu lateral esquerdo do Colab (ícone de pasta), faça o upload do arquivo `Space_Corrected.csv`.
5. Vá no menu superior do Colab e clique em **Ambiente de execução** -> **Executar tudo**.

---

##  Tecnologias de Código Utilizadas
* **Python 3**
* **Pandas:** Estruturação de DataFrames, tratamento de strings e cálculo das métricas.
* **NumPy:** Vetorização estatística.
* **Seaborn & Matplotlib:** Engenharia de eixos gráficos e renderização visual corporativa.

