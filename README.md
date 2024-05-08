# DESAFIO CIENTISTA DADOS GEO PECSMART

###Descrição do Problema:
Você foi contratado para atuar como cientista de dados geoespaciais e auxiliar no desenvolvimento de um sistema de otimização de calendário e rotas de envio de ração da fábrica para granjas produtoras de aves em uma determinada região de Santa Catarina. Tanto as granjas como a fabrica de ração serão equipadas com sensores IOT coletando informação sobre o estoque de ração, com atualizações diárias. Os dados atualizados serão disponibilizados diariamente para serem consumidos pelo algoritmo de roteirização, em formato parecido ao exemplo anexo ao desafio dados_desafio_rotas.xlsx.

### Requisitos do Sistema:
1. O sistema deve calcular a rota mais eficiente para entregar a ração em todas as granjas, minimizando a distância percorrida, garantindo a melhor eficiência na relação km rodado por kg entregue. Também deverá garantir que os caminhões saiam sempre cheios e retornem vazios para fábrica;
2. A entrada do sistema será um arquivo contendo as coordenadas geográficas (latitude e longitude) de cada granja e da fábrica de ração e seus respectivos estoques.
3. A saída do sistema deve ser a ordem de visitação das granjas e a distância total percorrida.

## Desafios:

### Desafio 1:
Proponha conceitualmente um modelo para desenvolvimento deste projeto, listando quais variáveis são importantes de serem consideradas, quais os principais desafios e quais modelos e tecnologias podem ser empregadas no seu desenvolvimento?

### Desafio 2:
Implemente script em Python (p.ex. utilizando Google Collab ou Jupyter) ou outra linguagem de preferência do candidato que leia um arquivo de entrada contendo as coordenadas geográficas das granjas e da fábrica de ração (dados_desafio_rotas.csv) e plote em um formato de mapa as posições das granjas e fábrica e seus respectivos estoques.
