#  Global Solution – Modelagem Linear para Aprendizagem de Máquina

##  Informações do Projeto

**Instituição:** FIAP – Faculdade de Informática e Administração Paulista  
**Curso:** Bacharelado em Ciência da Computação  
**Turma:** 1CCPJ  
**Disciplina:** Modelagem Linear para Aprendizagem de Máquina  
**Desafio:** Análise Estatística Aplicada à Nova Economia Espacial

###  Integrantes

- Maria Eduarda Rocha Benjamim – RM 570554
- Pedro Henrique Neves – RM 571382
- Akin Alexandre Mendes Martins – RM 572553

---

#  Objetivo do Projeto

Este projeto tem como finalidade aplicar técnicas de Estatística Descritiva, Distribuição de Frequências e Análise Exploratória de Dados para investigar padrões presentes no mercado aeroespacial mundial.

A análise foi desenvolvida a partir de dados históricos de missões espaciais, permitindo identificar tendências de crescimento do setor, comportamento dos custos operacionais e possíveis oportunidades associadas à chamada **Nova Economia Espacial (New Space Economy)**.

---

#  Base de Dados

## Origem

**Dataset:** All Space Missions from 1957  
**Arquivo Utilizado:** `Space_Corrected.csv`

**Fonte:** Kaggle – Space Missions Dataset

## Justificativa da Escolha

O conjunto de dados reúne informações reais sobre lançamentos espaciais realizados por governos e empresas privadas desde o início da exploração espacial moderna.

Sua utilização possibilita:

- Estudar a evolução histórica da atividade espacial;
- Analisar custos de missões ao longo do tempo;
- Identificar padrões de investimento;
- Aplicar técnicas estatísticas em dados reais de mercado.

Além disso, a base contém variáveis quantitativas e categóricas adequadas para análises exploratórias e modelagem estatística.

---

# Estrutura do Repositório

```text
├── README.md
├── Space_Corrected.csv
├── global_solution.ipynb
├── relatorio_final.pdf
```

## Descrição dos Arquivos

| Arquivo | Descrição |
|----------|------------|
| README.md | Documentação do projeto |
| Space_Corrected.csv | Base de dados utilizada |
| global_solution.ipynb | Notebook contendo o código-fonte da análise |
| relatorio_final.pdf | Relatório estatístico final |

---

#  Metodologia

O projeto foi desenvolvido em Python utilizando o ambiente Google Colab.

## 1. Tratamento dos Dados

Foram realizadas as seguintes etapas:

- Importação da base de dados;
- Limpeza de valores ausentes;
- Conversão dos custos das missões para formato numérico;
- Extração do ano de lançamento da variável temporal;
- Padronização dos dados para análise estatística.

## 2. Construção das Variáveis

### Variável Quantitativa Discreta

**Ano de Lançamento**

Utilizada para analisar a evolução histórica das missões espaciais.

### Variável Quantitativa Contínua

**Custo da Missão (USD Milhões)**

Utilizada para avaliar a distribuição dos investimentos no setor espacial.

---

## 3. Tabelas de Distribuição de Frequência

Foram construídas tabelas contendo:

- Frequência Absoluta (fi)
- Frequência Acumulada (Fi)
- Frequência Relativa (%)

para ambas as variáveis analisadas.

---

## 4. Estatística Descritiva

Foram calculadas as seguintes medidas:

### Medidas de Tendência Central

- Média
- Mediana
- Moda

### Medidas de Dispersão

- Variância
- Desvio Padrão
- Amplitude

### Medidas Separatrizes

- Quartil 1 (Q1)
- Quartil 2 (Q2)
- Quartil 3 (Q3)

---

## 5. Visualização de Dados

Foram produzidos gráficos utilizando Matplotlib e Seaborn:

### Gráfico Temporal

Evolução do número de lançamentos ao longo dos anos.

### Histograma com KDE

Distribuição dos custos das missões espaciais.

---

#  Principais Resultados

## Crescimento da Atividade Espacial

Os dados mostram um aumento significativo da quantidade de lançamentos nas décadas mais recentes, evidenciando a expansão do setor espacial comercial.

## Concentração de Custos

A maior parte das missões encontra-se nas faixas de menor custo, indicando redução das barreiras financeiras para entrada de novas empresas.

## Assimetria Positiva

A distribuição dos custos apresenta cauda à direita, caracterizando a existência de poucos projetos extremamente caros em comparação à maioria das missões.

## Faixa Predominante de Operação

Os quartis mostram que grande parte das missões está concentrada em níveis intermediários e baixos de investimento, reforçando a tendência de operações mais enxutas e escaláveis.

---

#  Conclusões

A análise estatística permitiu compreender melhor o comportamento econômico do setor espacial contemporâneo.

Os resultados evidenciam:

- Crescimento consistente da atividade espacial;
- Popularização de missões de menor custo;
- Forte influência da iniciativa privada no mercado;
- Necessidade de utilização de métricas robustas para modelagem preditiva devido à assimetria dos dados.

Esses achados reforçam a importância da Estatística e da Ciência de Dados como ferramentas estratégicas para tomada de decisão em mercados altamente tecnológicos.

---

#  Tecnologias Utilizadas

- Python 3
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

#  Como Executar

## 1. Clone ou baixe o projeto

```bash
git clone <url-do-repositorio>
```

## 2. Abra o Google Colab

Acesse:

https://colab.research.google.com

## 3. Faça upload dos arquivos

- `global_solution.ipynb`
- `Space_Corrected.csv`

## 4. Execute o notebook

No menu superior:

```text
Ambiente de Execução → Executar Tudo
```

## 5. Visualize os resultados

O notebook irá gerar automaticamente:

- Tabelas de frequência;
- Estatísticas descritivas;
- Gráficos exploratórios;
- Insights para análise da Nova Economia Espacial.

---

#  Referências

- Kaggle – All Space Missions from 1957 Dataset
- Pandas Documentation
- NumPy Documentation
- Matplotlib Documentation
- Seaborn Documentation

---

##  Licença

Projeto desenvolvido para fins acadêmicos na disciplina de Modelagem Linear para Aprendizagem de Máquina da FIAP.

---

**FIAP – Bacharelado em Ciência da Computação**  
**Global Solution 2026/1 – Modelagem Linear para Aprendizagem de Máquina**

OBSERVAÇÃO : Ferramentas de Inteligência Artificial foram utilizadas como apoio na organização, revisão e documentação deste projeto. Toda a implementação, análise dos dados e interpretação dos resultados foram realizadas e validadas pelos integrantes do grupo, que assumem total responsabilidade pelo trabalho apresentado.
O uso da IA teve caráter exclusivamente auxiliar, respeitando as diretrizes da FIAP para utilização responsável de tecnologias de apoio à aprendizagem.
