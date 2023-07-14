O Trabalho

O trabalho se dá acerca do jogo dos gradus de Kevin Bacon. Qualquer ator de Hollywood pode estar conectador a Kevin Bacon em até seis 
conexões de distâncias, os graus de bacon. Para saber o grau de bacon entre dois atores de Hollywood, é necessário encontrar o menor
caminho entre ambos. Existem duas bases de dados, nos diretórios small e large. 

Base de Dados
A base de dados possui movies.csv, people.csv e stars.csv . 

Movies.csv tem o id do filme, seu titulo e ano.
people.csv tem o id, o nome e o ano de nascimento dos atores
stars.csv relaciona o id do ator com o id do filme

degrees.py

names  = um dicionário guarda o id, tendo como chave o nome. Ou seja, buscando um nome, encontra-se um ou mais IDs.
people = um dicionário guarda um outro dicionaro com o nome da pessoa, o ano de nascimento e um set dos ids dos filmes.
movies = tem como chave o id do filme e guarda para cada um dicionário com valores para o filme, ano, titulo e id de todas as estrelas.


Todos os dados da base de dados são carregados com o método load_data 

A função main carrega todos os dados em memória, então dois nomes são perguntados no prompt. Primeiramente, o id destes nomes é consultado, 
consultando este nome em names, e pegando o id. O método que faz isso se chama person_id_for_name.

Tendo os ids das pessoas já de forma correta, devo então implementar shortest_path, para descobrir o grau de bacon do

Qual é a diferença entre este trabalho e Maze ou os fenícios ?

Bom, o percurso que pode ser percorrido é o seguinte:

 - Carregar todos os filmes que o ator fez
 - Para cada filme que ele fez:
	para cada filme
		carregar o filme
		para cada ator
			checar se ele é o destino
			se for 
				retornar
			se não for
				já está no frontier ?
					nada				
				não está no frontier ?
					adiciona ao frontier		
	
		