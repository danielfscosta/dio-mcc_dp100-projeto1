# Desafio de Projeto 1 - Prevendo Vendas de Sorvete com Machine Learning

## Proposta
Neste desafio de projeto busca-se, para um caso hipotético, o desenvolvimento de um modelo preditivo de Machine Learning para otimização da produção de sorvetes baseando-se na correlação entre vendas e temperatura ambiente.

## Resumo do projeto

- Inicialmente foi criado um prompt para geração através de uma IA Generativa de uma base de dados com os campos data, temperatura e vendas. Esta base de dados foi exportada em um arquivo ".csv";
- Fez-se necessária a criação de um novo grupo de recursos através do Azure portal para incluir todos os elementos utilizados na solução;

![image](src/img/dio-mcc_dp100-projeto1-01.png)
  
- No grupo de recursos criou-se um do tipo "Azure Machine Learning", que será útil na criação e implantação do modelo;

![image](src/img/dio-mcc_dp100-projeto1-02.png)

- Inicialmente no Azure Language Studio foi criado um novo "Asset" do tipo "Data" e importado o arquivo ".csv" com a base de dados;

![image](src/img/dio-mcc_dp100-projeto1-04.png)

- Para o processamento de treinamento execução do modelo foi criado um cluster de computação com duas instâncias do tipo Standard_DS11_v2 (2 cores, 14 GB RAM, 28 GB disk);

![image](src/img/dio-mcc_dp100-projeto1-03.png)

- Posteriormente foi criado um modelo para treinamento através do "Automated ML" e outro através do "Designer" utilizando algoritmos de regressão linear, tendo sido ambos implantados e executados;

![image](src/img/dio-mcc_dp100-projeto1-05.png)

![image](src/img/dio-mcc_dp100-projeto1-06.png)

![image](src/img/dio-mcc_dp100-projeto1-07.png)

- Após o término da execução, seguem os resultados encontrados, incluindo as métricas para o melhor modelo avaliado.

![image](src/img/dio-mcc_dp100-projeto1-08.png)

![image](src/img/dio-mcc_dp100-projeto1-09.png)
