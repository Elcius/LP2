							---- Projeto de LP2 Pt1 ----

	Esse projeto consiste na implementação em c++ de um programa, no qual dado um conjunto N de entradas (requisições), são geradas N respostas através de threads. Contém três diretórios: files, answ e reqs. Em reqs estão as requisições, em files os arquivos requisitados e em answ as respostas geradas.

	Caso as requisições possuam algum comando inválido é gerado uma resposta contendo "Erro: Comando invalido!". Para a requisição de um arquivo não existente é gerado um arquivo de resposta contendo "Erro: Arquivo requisitado não encontrado!". Todas as requisições estão no formato '.req' e todas as respostas no formato '.answ'.

	Para o tratamento da seção crítica temos uma trava, e para o encerramento em conjunto das threads temos uma barreira implementada. O programa encerra informando a quantidade total de bytes processados por todas as threads que foram criadas através da utilização da biblioteca threads.

-- Compilação:

	Para rodar o programa basta incluir os comandos: -pthread -std=c++11 no terminal.
