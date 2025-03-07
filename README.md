# Taxa de Mortalidade
Sobre o Projeto: Este projeto tem como objetivo analisar a taxa de mortalidade global ao longo dos anos, identificando padrões e tendências entre países e faixas etárias. Além disso, utilizei técnicas de Machine Learning para prever a taxa de mortalidade com base em variáveis como país, ano e gênero, fornecendo insights que podem auxiliar na formulação de políticas públicas e medidas preventivas.

# 📊 Questões Analisadas:

# Qual país tem a maior média de taxa de mortalidade por 100.000 indivíduos ao longo dos anos?

O código que ultilizei, converte a coluna Death Rate Per 100,000 para um formato numérico adequado, calcula a média da taxa de mortalidade para cada país, e, em seguida, identifica o país com a maior taxa média de mortalidade, bem como o valor dessa taxa, assim conseguindo identificar que: O país com a maior média de taxa de mortalidade é Mali com 16663.68 mortes por 100.000 indivíduos

# Qual é a tendência na taxa de mortalidade por 100.000 indivíduos ao longo dos anos para os países da América do Sul?

Realizei a filtragem de dados para países da América do Sul, assim calculei a taxa média de mortalidade por 100.000 habitantes para cada país e ano, e visualizei a tendência dessas taxas ao longo do tempo. A visualização foi feita por meio de um gráfico de linhas, onde cada linha representa um país da América do Sul. Este processo foi utilizado para análise comparativa das taxas de mortalidade na região, ajudando a identificar padrões ou mudanças ao longo dos anos. 

![image](https://github.com/user-attachments/assets/d6a589ee-c963-4fbb-a583-b297220068c1)

Ao gerar o gráfico, consegui identificar que a taxa de mortalidade está caindo ao longo do tempo, o que pode refletir melhorias nos cuidados de saúde, na qualidade de vida, nos avanços médicos, etc.


# Existem diferenças significativas nas taxas de mortalidade entre homens e mulheres em diferentes grupos etários na América do Sul?

Para resolver a questão eu dividi os dados de mortalidade entre homens e mulheres, criando dois subconjuntos: um para os homens e outro para as mulheres. Para cada grupo, calculei a taxa de mortalidade média por faixa etária, ou seja, analisei a taxa de mortes por 100.000 habitantes para diferentes faixas etárias, tanto para os homens quanto para as mulheres. Depois, organizei esses dados em um DataFrame mais claro, onde cada linha corresponde a uma faixa etária e contém as taxas de mortalidade tanto para homens quanto para mulheres, eu classifiquei as faixas etárias de forma sequencial, do grupo mais jovem ao mais velho. Por fim, criei um gráfico de linha para comparar visualmente as taxas de mortalidade entre homens e mulheres ao longo das diferentes faixas etárias. O gráfico me ajudou a identificar possíveis diferenças nas taxas de mortalidade entre os sexos em cada faixa etária, o que é importante para entender melhor como as condições de saúde e a mortalidade variam entre homens e mulheres na América do Sul.


![image](https://github.com/user-attachments/assets/c30d342d-48ac-447e-a18e-c6f203811022)

Ao gerar o gráfico ficou muito mais claro entender e visualizar que não existem diferenças significativas nas taxas de mortalidade entre homens e mulheres em diferentes grupos etários na América do Sul, a não ser com 0-6 dias de vida que vemos uma grande diferença.

# Como a taxa de mortalidade por 100.000 indivíduos varia entre diferentes grupos etários dentro do Brasil?

Neste código, eu analisei como a taxa de mortalidade por 100.000 indivíduos varia entre diferentes faixas etárias dentro do Brasil. Primeiro, filtrei os dados para considerar apenas o Brasil e converti a coluna "Número de Mortes" para um formato numérico, removendo as vírgulas. Depois, removi a faixa etária "All Ages" para focar nas faixas etárias específicas. Agrupei os dados por ano e faixa etária, calculando a média da taxa de mortalidade para cada grupo. Isso me permitiu ver como a taxa de mortalidade variava ao longo do tempo para diferentes faixas etárias. Por fim, criei um gráfico de barras para visualizar a distribuição das taxas de mortalidade por faixa etária no Brasil. O gráfico me ajudou a entender melhor como as taxas de mortalidade mudaram ao longo dos anos em cada faixa etária e identificar possíveis padrões ou tendências.

# Qual a evolução das mortes por gênero no Brasil?

Neste código, eu analisei a evolução das mortes por gênero no Brasil ao longo dos anos. Para isso, comecei filtrando os dados para considerar apenas as informações do Brasil. Em seguida, converti a coluna "Número de Mortes" para o formato numérico, removendo as vírgulas, o que me permitiu trabalhar corretamente com os dados.Depois, agrupei os dados por ano e gênero e calculei o total de mortes para cada gênero, somando as mortes de homens e mulheres a cada ano. Utilizei o método .unstack() para transformar os dados de forma que cada gênero fosse representado em uma coluna separada.

![image](https://github.com/user-attachments/assets/55d7b971-1641-4868-bcd0-ce1b03fb2db9)

Por fim, criei um gráfico de linhas, onde cada linha representa a evolução das mortes por um dos gêneros (masculino e feminino) ao longo dos anos. O gráfico me ajudou a visualizar como as mortes no Brasil variaram por gênero entre 1970 e 2010, permitindo uma análise clara da evolução ao longo do tempo.

# Qual grupo etário tem o maior número de mortes no Brasil? Esse número é o mesmo ao longo de todos os anos ou houve mudanças nos últimos 10 anos?

Neste código, eu analisei qual grupo etário tem o maior número de mortes no Brasil, comparando os dados de todos os anos com os últimos 10 anos (2000-2010). Primeiro, agrupei os dados por grupo etário para todos os anos (1970-2010) e calculei o total de mortes por grupo etário, ordenando os resultados de forma decrescente. Isso me permitiu identificar qual grupo etário teve o maior número de mortes no Brasil durante todo o período. Em seguida, filtrei os dados para considerar apenas os últimos 10 anos (2000-2010) e repeti o processo de agrupamento e soma de mortes por grupo etário. Com isso, pude comparar os resultados e verificar se o grupo etário com o maior número de mortes foi o mesmo nas duas análises (todos os anos versus apenas os últimos 10 anos).

Ao imprimir os resultados, percebi que, para o período de 1970 a 2010, o grupo "80+ years" teve o maior número de mortes, enquanto para os últimos 10 anos (2000-2010), o grupo "80+ years" também liderou, mas a quantidade de mortes foi significativamente menor do que no período completo.


# Qual país apresentou a maior melhoria nas taxas de mortalidade ao longo dos anos?

Neste código, eu analisei qual país apresentou a melhoria mais significativa nas taxas de mortalidade por 100.000 indivíduos ao longo do período de 1970 a 2010. Primeiro, transformei os dados da coluna "Death Rate Per 100,000" para um formato numérico adequado, removendo as vírgulas. Em seguida, agrupei os dados por país e ano e calculei a média das taxas de mortalidade para cada país em 1970 e 2010. Com isso, calculei a diferença nas taxas de mortalidade entre esses dois anos para cada país, o que me permitiu medir a melhoria (ou piora) nas taxas de mortalidade ao longo do período analisado.

Por fim, encontrei o país que apresentou a maior melhoria na taxa de mortalidade, ou seja, a maior redução nas mortes por 100.000 habitantes. O país com a maior melhoria foi as Maldivas, com uma redução de 15.301,04 mortes por 100.000 habitantes de 1970 a 2010.

Esse processo me ajudou a identificar os países que mais avançaram na redução das taxas de mortalidade ao longo do tempo.


# Insights Importantes:

📌Diferenças nas Taxas de Mortalidade por Países da América do Sul:

Ao analisar a taxa de mortalidade por 100.000 indivíduos ao longo dos anos para os países da América do Sul, foi possível observar tendências e padrões diferentes entre os países. Todos os países mostraram uma redução significativa nas taxas ao longo do tempo. Esse comportamento pode estar relacionado a fatores como políticas de saúde pública, acesso a cuidados médicos e condições econômicas.

📌Diferença na Taxa de Mortalidade entre Homens e Mulheres:

A análise da taxa de mortalidade por faixa etária entre homens e mulheres revelou diferenças claras, com algumas faixas etárias mostrando taxas de mortalidade significativamente mais altas para homens em comparação com as mulheres. Esse tipo de análise é crucial para entender a desigualdade de gênero nas taxas de mortalidade e pode ajudar a identificar necessidades específicas em termos de políticas de saúde para homens e mulheres em diferentes faixas etárias.

📌Evolução das Mortes no Brasil:

Ao traçar a evolução das mortes por gênero no Brasil ao longo dos anos, foi possível perceber mudanças nas taxas de mortalidade entre homens e mulheres. Esse tipo de análise pode ser útil para políticas de saúde pública, pois permite entender como a mortalidade tem se comportado por gênero e como diferentes fatores podem ter impactado essas taxas ao longo do tempo.

📌Grupo Etário com Maior Número de Mortes no Brasil:

A análise das mortes por faixa etária no Brasil revelou que o grupo "80+ years" apresentou o maior número de mortes ao longo do período de 1970 a 2010, refletindo o envelhecimento da população e o impacto de doenças crônicas e comorbidades associadas à idade avançada.

No entanto, ao olhar para os últimos 10 anos (2000-2010), a distribuição de mortes ainda se concentra em faixas etárias mais avançadas, mas o impacto de outras faixas etárias, como 70-74 anos e 75-79 anos, também se mostrou significativo. Esse insight destaca a importância de direcionar recursos e políticas de saúde para as faixas etárias mais vulneráveis, especialmente à medida que a população envelhece.

📌País com Maior Melhoria nas Taxas de Mortalidade:

As Maldivas se destacaram como o país com a maior melhoria nas taxas de mortalidade por 100.000 habitantes entre 1970 e 2010, com uma redução impressionante de 15.301,04 mortes. Esse dado sugere que as Maldivas implementaram políticas de saúde pública eficazes ao longo desse período, o que pode ter incluído melhorias em infraestrutura médica, prevenção de doenças e aumento do acesso a cuidados de saúde.

Esse insight pode ser importante para outros países que buscam melhorar suas taxas de mortalidade, uma vez que as Maldivas podem servir como um modelo de boas práticas para redução de mortes por doenças evitáveis.

📌Análise Temporal e Geográfica:

Ao comparar as taxas de mortalidade ao longo do tempo e entre diferentes países, é possível notar que há grandes variações regionais e temporais. Por exemplo, enquanto alguns países da América do Sul mostraram quedas nas taxas de mortalidade, outros ainda apresentam aumentos ou estagnação. 

A análise temporal mostra que ao longo das décadas houve avanços significativos, mas também desafios persistentes, como as taxas de mortalidade em faixas etárias mais altas.

📌Impacto das Faixas Etárias nas Taxas de Mortalidade:

A variação nas taxas de mortalidade entre diferentes faixas etárias indica que políticas de saúde pública devem ser cada vez mais segmentadas por faixa etária. Para países com populações envelhecendo, como o Brasil, as faixas etárias mais avançadas precisam de um foco particular, considerando que são as mais impactadas pelas altas taxas de mortalidade. Isso inclui estratégias para enfrentar doenças crônicas e melhorar a saúde do idoso.

# 🛠 Machine Learning

Como parte da análise, desenvolvi um modelo preditivo baseado em Regressão Linear com o objetivo de estimar a taxa de mortalidade considerando variáveis como país, ano e gênero.

# Como o modelo funciona?

Pré-processamento dos Dados:

Inicialmente, foi realizado o tratamento de valores ausentes para garantir a integridade dos dados. Em seguida, os dados foram normalizados, visando melhorar a performance do modelo. Para lidar com as variáveis categóricas (país e gênero), apliquei a técnica de OneHotEncoding, convertendo essas variáveis em valores numéricos que pudessem ser processados pelo modelo.

Criação do Modelo:

Utilizei um modelo de Regressão Linear, que foi treinado para identificar e estabelecer relações entre as variáveis independentes e a taxa de mortalidade.
O conjunto de dados foi dividido em 80% para treino e 20% para teste, garantindo que o modelo fosse capaz de generalizar para dados não vistos anteriormente.

Avaliação do Modelo:

Para medir a performance do modelo, utilizei o Erro Quadrático Médio (MSE), que avalia a precisão das previsões feitas pelo modelo.
Embora o modelo tenha apresentado um desempenho razoável, explorei possíveis melhorias, como o uso de modelos mais complexos, como Random Forest e XGBoost, que podem gerar resultados mais robustos e precisos.

# Resultado do Modelo:

O erro médio do modelo foi 17.714.368.548,85, o que indica que, embora o modelo tenha conseguido capturar tendências gerais nas taxas de mortalidade, sua precisão ainda pode ser aprimorada. O modelo mostrou-se eficaz para prever tendências, mas melhorias podem ser alcançadas ao incorporar abordagens mais avançadas de Machine Learning, o que proporcionaria previsões mais precisas e confiáveis.

Este trabalho serve como um ponto de partida para a aplicação de modelos preditivos no contexto de mortalidade, e evidencia a necessidade de explorar técnicas mais avançadas para um melhor desempenho.

# Conclusão

Este projeto possibilitou uma análise detalhada dos dados de mortalidade global, permitindo a identificação de padrões e tendências significativas. Através dessa análise, foi possível explorar a evolução da mortalidade ao longo do tempo e entender fatores que contribuem para essas variações.

# Algumas descobertas importantes :

Disparidade entre a mortalidade de homens e mulheres: Foi observada uma diferença nas taxas de mortalidade por gênero, com alguns grupos etários apresentando taxas mais altas para um dos sexos. Esta disparidade aponta para a necessidade de políticas de saúde pública mais específicas para cada gênero.

Tendência de queda em alguns países e estagnação em outros: Alguns países apresentaram uma redução contínua nas taxas de mortalidade, enquanto outros mostraram estagnação ou até aumento das taxas. Esses comportamentos podem estar associados a diferentes estratégias de saúde pública, desenvolvimento econômico e acesso a serviços médicos.

Melhoria significativa em certas regiões devido a políticas públicas eficientes: A análise revelou que países como as Maldivas obtiveram uma redução substancial nas taxas de mortalidade, o que pode ser atribuído a políticas públicas eficazes, como melhorias na infraestrutura de saúde, prevenção de doenças e cuidados médicos.

O modelo de Machine Learning ainda pode ser aprimorado: Embora o modelo preditivo tenha sido útil para analisar os dados, ele pode ser otimizado com o uso de algoritmos mais avançados, o que resultaria em previsões mais precisas e robustas. A melhoria contínua do modelo pode oferecer insights ainda mais profundos sobre as tendências de mortalidade global.

Este estudo serve como um ponto de partida para o entendimento das dinâmicas de mortalidade e reforça a importância de se continuar investindo em análises mais detalhadas e modelos preditivos mais avançados.
