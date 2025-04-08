Matheus Henrique Moreno da Silva
Professor: Douglas Dionizeti de Castilho Braz
Materia: Projeto e Analise de Algoritmos

Ultimo trabalho pratico da disciplina de PAA, onde devemos planejar 
o que cozinhar nos proximos dias, onde se um prato é cozinhado duas
vezes seguidas, o valor do lucro na segunda vez é de 50% do lucro na primeira vez
 se é preparado uma terceira vez seguida, o valor do lucro é zero.
 A entrada consiste em varios casos de teste, comecandl com 3 inteiros em uma linha:
 o numero de dias k (1<= k <= 21), o numero de pratos n(1<=n<50) que ele pode cozinhar
 e seu orçamento m (0<= m <= 100).

 A solução abordada pode ser descrita pela relação entre o lucro e venda, 
 tal que R = L/P, podemos ordenar essa relação buscando o melhor lucro em relação
  ao preço, assim nos resta buscar a melhor combinação. Apesar de fazer muitas comparações
  pode afirmar que a solucao é proximo do otimo.
  Foi adaptado um algoritmo guloso(Greedy), onde busca resolver problemas complexos, com a melhor relação possivel.
  No caso apresentado busca a melhor relação entre lucro e preço.

Na função resultado, recebemos a lista de vendas, lucro, a quantidade de pratos, a quantidade de dias e a quantidade de dinheiro
disponivel.
O HashMap "valorPorLucro", é criado para associar cada valor de lucro por preço a um valor de prato.
Duas listar para armazenar valores ordenados, "valorPLucroSorted" e "lucroA"