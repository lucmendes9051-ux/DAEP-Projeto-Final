# ⚙️ Análise de Desempenho Operacional na Manufatura

Projeto de análise exploratória de dados focado no desempenho operacional de uma fábrica industrial. O objetivo é analisar tempos de produção, paradas e reprocessos, gerando insights estratégicos para a Engenharia de Produção.

##  Dataset

* **Arquivo:** `Data/project_Manufacturing Dataset.csv`
* **Fonte:** [Manufacturing Dataset – Kaggle](https://www.kaggle.com/)
* **Registros:** 3.000 ordens de produção
* **Período Analisado:** Janeiro 2020 a Março 2020 (Amostra)

### Colunas principais utilizadas na análise

| Coluna | Descrição |
| :--- | :--- |
| `Date` | Data do registro de produção |
| `Product Type` | Tipo de produto (Appliances, Automotive, Electronics, Textiles) |
| `Shift` | Turno de trabalho (Day, Night, Swing) |
| `Production Time Hours` | Horas de produção efetiva |
| `Maintenance Hours` | Horas gastas com manutenção do maquinário |
| `Down time Hours` | Horas de máquina parada (inatividade) |
| `Rework Hours` | Horas gastas em reprocesso de peças com defeito |



##  Estrutura de Arquivos

```text
DAEP-Projeto-Final/
├── Data/
│   └── project_Manufacturing Dataset.csv  # Dataset bruto
├── projeto.ipynb                          # Notebook principal com a análise executável
└── README.md                              # Documentação do projeto
```
### Como Executar
Pré-requisitos: Instalar as dependências no ambiente virtual do projeto:

Bash
pip install pandas matplotlib

### Opção 1 — Jupyter Notebook
1. Iniciar o servidor (jupyter notebook).

2. Abrir o ficheiro projeto.ipynb e executar todas as células (Cell > Run All)

### Estrutura do Notebook (projeto.ipynb)
Seção 1 — Exploração e Importação dos Dados
Importação das bibliotecas, carregamento do CSV e análise inicial ("Raio X") das colunas, tipos de dados e contagem de valores nulos.

Seção 2 — Limpeza e Preparação
Filtro das 17 colunas estritamente relacionadas ao desempenho e tratamento de aproximadamente 300 valores nulos nas colunas de gargalo (Maintenance Hours, Rework Hours, etc.) utilizando a mediana, evitando a distorção da análise por outliers.

Seção 3 — Resumo Estatístico
Geração de métricas descritivas (média, desvio padrão, min, max). Agrupamento dos dados de tempo de parada por turno utilizando a função groupby().
