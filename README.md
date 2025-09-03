# **Projeto de Análise de Manutenção Industrial com Databricks e SQL**

## **Visão Geral**

Este projeto é um portfólio de análise de dados com foco em manutenção industrial, desenvolvido para demonstrar habilidades em **engenharia de dados**, **SQL avançado** e **visualização**. A solução proposta aborda o desafio de otimizar a manutenção de equipamentos, transformando dados brutos em insights acionáveis para melhorar a eficiência e a confiabilidade das operações.

### **O Problema de Negócio**

Em um ambiente industrial, falhas de máquinas e ociosidade não planejada geram perdas de produtividade e aumento de custos. A manutenção reativa, que age apenas após a ocorrência de uma falha, é ineficiente. Este projeto busca mudar esse cenário, utilizando a análise de dados para migrar de um modelo reativo para um modelo proativo, baseado em dados.

## **Tecnologias Utilizadas**

- **Databricks Community Edition:** Ambiente de desenvolvimento e processamento de dados em larga escala.
- **SQL (Spark SQL):** Linguagem principal para ETL, análise e cálculo de KPIs.
- **Unity Catalog:** Solução de governança de dados do Databricks, utilizada para organizar e gerenciar as tabelas.
- **Delta Lake:** Formato de armazenamento que garante a confiabilidade e a integridade dos dados.

## **Metodologia do Projeto**

A metodologia seguiu um pipeline de dados completo, simulando um ambiente de produção real.

1. **Engenharia de Dados (Pipeline Raw to Gold):** Os dados brutos de ocorrências de falhas, informações de máquinas e planos de manutenção foram processados para uma tabela "gold" (pronta para análise). Nessa etapa, a duração das paradas e a gravidade das falhas foram calculadas e adicionadas, enriquecendo a base para a análise posterior.
2. **Análise de Dados Avançada:** A tabela "gold" foi utilizada para calcular e analisar métricas-chave de desempenho (KPIs) da manutenção.
3. **Visualização:** Os resultados das análises foram visualizados em gráficos, facilitando a interpretação e a comunicação dos insights.

## **Análises e Resultados (KPIs)**

As análises aprofundadas revelaram insights importantes para a gestão da manutenção:

### **1\. Confiabilidade e Eficiência (MTBF e MTTR)**

O **MTBF (Tempo Médio Entre Falhas)** mede a confiabilidade dos equipamentos, enquanto o **MTTR (Tempo Médio para Reparo)** mede a eficiência da equipe de manutenção. A análise mostrou que:

- Máquinas com menor **MTBF**, como o **Torno CNC 2000**, são menos confiáveis e devem ser priorizadas para inspeções ou manutenções preventivas mais frequentes.
- A eficiência da equipe varia significativamente dependendo da causa da falha, indicando a necessidade de treinamento e recursos específicos para os reparos mais demorados.

### **2\. Causas de Falha e Impacto**

A análise das causas de falha por seu impacto total (combinando frequência e tempo de parada) é crucial para priorizar as ações de manutenção. As principais causas de parada foram:

- **Falha no sistema de refrigeração** e **Falha no rolamento**, que, embora não sejam as mais frequentes, geraram um tempo de ociosidade considerável.
- O estudo de impacto permite focar em resolver os problemas que mais prejudicam a produtividade.

### **3\. Análise de Tendência Mensal**

O acompanhamento dos KPIs ao longo do tempo (mês a mês) revelou tendências importantes:

- O **MTTR** variou em diferentes meses, mostrando que a eficiência da equipe de manutenção pode ser influenciada por fatores como carga de trabalho e complexidade das falhas.
- O aumento no número de falhas em determinados meses pode indicar sazonalidade ou gargalos na operação.

### **4\. Adesão ao Plano de Manutenção**

A análise da adesão ao plano de manutenção preventiva mostrou que:

- Embora a maioria das manutenções seja executada, há um percentual significativo de tarefas **atrasadas** ou **canceladas**.
- A correlação entre o status da manutenção preventiva e o aumento de falhas corretivas é um ponto chave para melhorar a estratégia de manutenção.

## **Lições Aprendidas e Próximos Passos**

Este projeto demonstrou a importância de um pipeline de dados bem estruturado para uma análise eficaz. A utilização de uma tabela "gold" centralizou a lógica de negócios, facilitando análises subsequentes e garantindo a consistência dos resultados. A experiência prática com Databricks e Unity Catalog provou ser imprescindivel para a governança e a escalabilidade dos dados.

Para evoluir este projeto, os próximos passos seriam:

- **Análise Preditiva:** Integrar dados de sensores (IoT) e construir modelos de Machine Learning para prever falhas antes que elas ocorram, transformando o projeto em uma solução de **manutenção preditiva**.
- **Análise de Custos:** Adicionar dados financeiros para calcular o **custo total da manutenção** por máquina e falha, além do Retorno sobre o Investimento (ROI) de iniciativas de manutenção preventiva.
- **Dashboard Interativo:** Criar um painel de controle interativo usando ferramentas de BI (como Power BI ou Tableau), permitindo que gestores de manutenção monitorem os KPIs em tempo real e tomem decisões proativas baseadas em dados.


### Autor

* **Nome:** André Cruz
* **LinkedIn:** andreluisdacruz
* **GitHub:** andreluisdacruz
* **Portifólio:** [Portifólio](https://sites.google.com/view/dacruzandre/p%C3%A1gina-inicial)
* **E-mail:** dacruzandreluis@gmail.com
