# Taxa_Mortalidade
 Sobre o Projeto: Este projeto tem como objetivo analisar a taxa de mortalidade global ao longo dos anos, identificando padrões e tendências entre países e faixas etárias. Além disso, utilizei técnicas de Machine Learning para prever a taxa de mortalidade com base em variáveis como país, ano e gênero, fornecendo insights que podem auxiliar na formulação de políticas públicas e medidas preventivas.

 Questões Analisadas:

Qual país tem a maior média de taxa de mortalidade por 100.000 indivíduos ao longo dos anos?

Identifiquei os países com maior taxa média e analisei os possíveis fatores que influenciam esses números.

Qual é a tendência na taxa de mortalidade por 100.000 indivíduos ao longo dos anos para os países da América do Sul?

Criei um gráfico de linhas exibindo a evolução das taxas de mortalidade para cada país da América do Sul.

Existem diferenças significativas nas taxas de mortalidade entre homens e mulheres em diferentes grupos etários na América do Sul?

Analisei as taxas de mortalidade separadas por gênero e idade, observando se há discrepâncias significativas.

Como a taxa de mortalidade por 100.000 indivíduos varia entre diferentes grupos etários dentro do Brasil?

Utilizei histogramas para visualizar a distribuição da taxa de mortalidade em diferentes faixas etárias.

Qual a evolução das mortes por gênero no Brasil?

Criei um gráfico de linhas para cada gênero, mostrando como a taxa de mortalidade evoluiu ao longo dos anos.

Qual grupo etário tem o maior número de mortes no Brasil? Esse número é o mesmo ao longo de todos os anos ou houve mudanças nos últimos 10 anos?

Analisei qual faixa etária apresenta maior mortalidade e se esse padrão se mantém ao longo do tempo.

Qual país apresentou a maior melhoria nas taxas de mortalidade ao longo dos anos?

Identifiquei os países que conseguiram reduzir significativamente suas taxas de mortalidade e discutimos os possíveis fatores responsáveis por essa melhoria.


Insights Importantes:

O país com a maior média de taxa de mortalidade foi Mali.

O Brasil apresentou uma tendência de queda na taxa de mortalidade nos últimos anos.

Em geral, as taxas de mortalidade são maiores para homens do que para mulheres em quase todas as faixas etárias.

O grupo etário mais afetado no Brasil foram pessoas com mais de 80 anos.

O país que obteve a maior melhoria na taxa de mortalidade ao longo dos anos foi Maldivas com uma redução de 15301.04 mortes por 100.000 habitantes.


Machine Learning

Para complementar a análise, desenvolvemos um modelo preditivo de Regressão Linear para estimar a taxa de mortalidade com base em país, ano e gênero.

 Como o modelo funciona?

Pré-processamento dos dados:

Lidamos com valores ausentes e normalizamos os dados.

Aplicamos OneHotEncoding para transformar variáveis categóricas (país e gênero) em valores numéricos.

Criação do modelo:

Utilizamos um modelo de Regressão Linear para encontrar relações entre as variáveis e a taxa de mortalidade.

Dividimos o conjunto de dados em 80% para treino e 20% para teste.

Avaliação do modelo:

Utilizamos Erro Quadrático Médio (MSE) para medir a precisão do modelo.

Analisamos possíveis melhorias no modelo, como o uso de modelos mais complexos (Random Forest, XGBoost, etc.).

 Resultado do modelo

O erro médio do modelo foi 17714368548.852146 , indicando qualidade da previsão, razoável. O modelo conseguiu prever tendências gerais, mas há espaço para melhorias, como o uso de abordagens mais avançadas de Machine Learning.


Conclusão

Este projeto permitiu uma exploração aprofundada dos dados de mortalidade global e o desenvolvimento de um modelo preditivo para entender padrões e tendências.

Algumas descobertas importantes incluem:

A disparidade entre a mortalidade de homens e mulheres.

A tendência de queda em alguns países e a estagnação em outros.

A melhoria significativa em certas regiões devido a políticas públicas eficientes.

O modelo de Machine Learning ainda pode ser aprimorado com algoritmos mais avançados para melhorar a precisão das previsões.
