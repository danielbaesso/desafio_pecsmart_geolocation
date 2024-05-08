# Modelo de Desenvolvimento 

Para desenvolver o projeto de otimização de rotas de entrega de ração para granjas, é importante considerar diversos aspectos e variáveis. Aqui está uma proposta conceitual para o modelo de desenvolvimento, destacando variáveis importantes, principais desafios e tecnologias/modelos que podem ser empregados: 

Conceituamente utilizou-se o problema do caixeiro viajante (Traveling Salesman Problem – TSP) que é um dos problemas mais clássicos da matemática. Ele consiste em se encontrar um percurso de comprimento mínimo, partindo de um dado local de início, visitando um conjunto de pontos na melhor ordem possível, e retornando ao local de origem, utilizando para isso somente os caminhos existentes que ligam esses pontos, ou seja baseado na teoria de graphos. 

A grande dificuldade encontrada em se resolver este problema se dá devido ao fato de que a dificuldade do problema cresça com o número de nós no grafo em questão. 

Durante este desafio buscou a resolução de forma simples, enxuta e direta. Criou-se o `Índice de Eficiência`, onde procurou encontrar uma relação entre a demanda da Granja e a distância desta até a Fábrica. Sendo assim quanto maior este índice maior a prioridade de atendimento desta Granja, já que representava que estava mais distante e com menor estoque em seus silos. Para esta análise podemos elencar: 


### Variáveis Importantes: 

*Localização das Granjas*: Latitude e longitude de cada granja. 

*Estoque de Ração nas Granjas*: Quantidade de ração disponível em cada granja. 

*Demanda de Ração das Granjas*: Quantidade de ração necessária por cada granja. 

*Distância entre Locais*: Distâncias em quilômetros entre a fábrica e as granjas, bem como entre as próprias granjas. 

*Eficiência de Entrega*: Índice de eficiência que leva em conta a distância percorrida e a quantidade de ração entregue. 

*Rota*: Informação detalhada sobre o trajeto a ser percorrido. (a ser calculada em um cenário real) 

*Veículo*: Informação sobre a capacidade e quantidade de veículos para a entrega. (a ser calculada em um cenário real) 


### Principais Desafios: 

*Otimização de Rotas*: Encontrar a combinação mais eficiente de granjas a serem atendidas em cada rota, minimizando a distância percorrida e maximizando a quantidade de ração entregue. 

*Gestão de Estoque*: Garantir que as granjas sejam abastecidas de acordo com sua demanda e que o caminhão seja o mais eficiente durante a entrega para garantir agilidade e economia. 

*Limitação de Recursos*: Considerar a capacidade do caminhão e a quantidade total de ração disponível na fábrica. 


### Modelos e Tecnologias: 

*Modelagem de Dados*: Utilização de DataFrames do pandas para manipulação e análise dos dados. 

*Cálculos de Distância*: Uso de bibliotecas como Haversine e Geopy para cálculos de distância entre locais. 

*Visualização de Mapas*: Utilização da biblioteca Folium para visualização interativa de mapas. 


### Desafios para o futuro 

*Otimização de Rotas*: Aplicação de algoritmos de otimização, como o Algoritmo do Caixeiro Viajante (TSP), através de bibliotecas como OR-Tools. 

*Interface de Usuário*: Desenvolvimento de uma interface para interação com o sistema, utilizando tecnologias web como Flask para o back-end e HTML/CSS/JavaScript para o front-end. 

*Sensoriamento Remoto*: Recebimento de informação automático e em tempo real via satélite.  


A abordagem geral seria coletar e organizar os dados das granjas e da fábrica, realizar cálculos de distância e eficiência, otimizar as rotas de entrega utilizando algoritmos apropriados e, por fim, visualizar as rotas otimizadas em um mapa interativo para facilitar a tomada de decisões. 