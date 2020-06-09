# Projeto de formacao Data Science

Caso queria executar esse notebook no seu computador, se o sistema operacional for windows, apenas execute o arquivo **StartJupyter** 
e espere uma aba abrir no seu navegador.Caso seja de distribuição Linux, rode o comando ```jupyer-notebook``` no diretório local de download deste projeto no seu computador.

## Situação problema

Você foi contratado para ajudar uma produtora de filmes a explorar informações sobre diversos generos de filmes. A ideia é obter 
informações sobre avaliações, popularidade, data de produção e gênero dos filmes.


Nesse seu primeiro trabalho como data scientist seu objetivo é fazer uma análise exploratória desse conjunto de dados.


## Bibliotecas utilizadas

* Pandas
* Seaborn
* Scipy
* Matplotlib

## Testes de normalidade

* Andreson: avalia qual tipo de distribuição os dados se comportam, retorna vários valores além do valor p. 
* Shapiro-Wilk: avalia se as amostra se comportam em uma gaussiana, boa para um pequeno conjunto de amostras.
* D'Agostino ou K² teste: retorna um remuso estatístico dos dados.

## Alguns pontos sobre o projeto

* A distribuições apresentadas como notas médias ou total de votos de um determinado gênero, algumas delas podem parecer uma distribuição 
gaussiana com skewness diferente de zero e curtose diferente da mesocúrtica, mas os testes estátisticos mostrados acima com a biblioteca scipy mostraram quase nenhuma dessas
distribuições eram gaussiana.

* Há filmes com mais de uma categoria, isso pode acarretar em contagem de votos um pouco mais do que outras, além disso, algumas categorias podem ter quantidade de votos
muito próximas, como é o caso de filmes de drama e ação, ou seja, se você está vota em um filmes pode está votando em duas ou mais categorias.

* Se dividirmos a quantidade de votos pela a quantidade de filmes resulta em que filmes de guerra tem o maior valor, isso traz muitas conclusões, como 
que há poucos filmes e muito votos neles, logo, isso pode mostrar um interesse dos usuários por esses tipos de filmes. Com isso, categoria guerra de filmes é mais facil de 
se encaixar com outras categorias, ou seja, é mais facil ver uma filmes rotulado como guerra/romance ou guerra/drama do que documentário/romance.

* Houve algo a partir da década de 1990 que a produção de filmes em todos os genêros aumentou, com isso, foi preciso analisar a correlação entre as colunas ou parâmetros
dividindo as amastros antes e depois desta época.

* Com base no total de votos, os filmes mais assistir a partir da década de 1990 são os de drama seguidos por uma pequena diferença a 
categoria de ação. Jás os filmes de comédia ficou na liderança antes da década de 1990(mas é claro, há muito mais filmes após essa época) seguindo também por uma pequena
diferenças os filmes de ação.
