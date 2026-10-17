Markdown
# Análise de Desempenho Operacional

Projeto final de análise de dados do setor industrial utilizando Python. O foco deste trabalho é analisar o **Desempenho Operacional** da fábrica, identificando gargalos nos tempos de produção, paradas e manutenção.

## 📁 Arquivos do Projeto

*   `project_Manufacturing Dataset.csv`: Base de dados original (3.000 registros).
*   `projeto.ipynb`: Jupyter Notebook contendo todo o código da análise, gráficos e insights.

## 🛠️ Tecnologias Utilizadas

*   **Python 3**
*   **Pandas:** Para limpeza, tratamento de dados nulos (usando mediana) e agrupamentos estatísticos.
*   **Matplotlib:** Para visualização gráfica dos ofensores de tempo.

## 📊 Estrutura da Análise

Nossa análise no notebook está dividida em:
1. **Exploração e Importação:** Carregamento do dataset.
2. **Limpeza e Preparação:** Filtro das 17 colunas de interesse e tratamento de valores nulos.
3. **Resumo Estatístico:** Análise descritiva e avaliação do tempo de parada por turno.
4. **Visualizações:** Histograma de horas de produção e Boxplot comparativo de gargalos.
5. **Insights e Conclusão:** Diagnóstico apontando a manutenção como principal ofensor de tempo e recomendação de manutenção preditiva.