# Azure Machine Learning


Neste repositótio armazeno o relatório final da Pós-Graduação em Data Science & Business Analytics realizada no ISEG, Universidade de Lisboa.

## O Projeto

O projeto consistia em criar uma solução à qual faríamos a ingestão dos dados de algum respositório Web, salvá-lo em um Data lake e posteriormente criar um relatório em Power Bi e por último o modelo de Machine Learning no Azure.

### Problema de Negócio

Antes de qualquer decisão eu e meu colega decidimos por utilizar dados de uma farmacéutica para realizar previsão de Churn de clientes.

### Estrutura Final

- Fonte dos dados: Os dados foram disponibilizados em um repositório no GitHub;
- Orquestrador do ETL: Foi utilizado o Azure Data Factory através de Pipelines para realizar a ingestão e transformações dos dados;
- Data Lake: O dados raws foram armazenados em Azure Data Lake em uma instância Raw, e de acordo do estado de processamento os dados os dados foram avançando de instâncias criadas para esses fins;
- Data Warehouse: Após todas as transformações os dados foram disponibilizados em um Azure Data Warehouse à qual criamos para armazenar os dados processados;
- SSAS: Utilizamos o SQL Server Analisys Services para ligar-se o Data Warehouse e criar um modelo tabular e construir a nossa camada semântica, model star, algumas measures, colunas e tabelas, ou seja, aqui fizemos o enrequecimento dos nossos dados;
- Power BI: Nesta etapa utilizamos o Power Bi em modo live connection à qual conecta diretamente ao SSAS e assim conseguimos fazer uso dos dados e criar alguns reports que serviu de base para conhecer melhor os nossos dados e auxiliar na tomada de decisão;
- Azure Machine Learning: Em último passo, utilizamos o AZML para criar nosso modelo de previsão de Churn, fizemos todas as etapas e testamos vários modelos com inúmeras modificações nos dados. Assim, no final após todos os testes conseguimos construir um modelo que pudesse resultar de boas métricas.

Caso tenham qualquer dúvida ou sugestão, basta entrar em contato.
