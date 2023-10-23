# M2S05 - Atividades SQL

### [M02S05] Ex 01 - Copa do Mundo (parte 1) - Tabela de Times

Neste ano de 2022 vai acontecer a Copa do Mundo de Futebol no Qatar!

Pra ajudar a organização do campeonato, vamos montar um banco de dados dos times participantes!

a) Criar uma tabela chamada TIMES com os campos 'sigla' (varchar e chave primária) e 'nome' (varchar e não-nulo).
b) Inserir nesta tabela os times participantes da Copa, conforme listagem mais abaixo.
c) Consultar todos os itens da lista para conferir o registro de todas as linhas.

## SIGLA - NOME

QAT - Qatar
ECU - Equador
SEN - Senegal
NED - Holanda
ENG - Inglaterra
IRN - Irã
USA - Estados Unidos
WAL - País de Gales
ARG - Argentina
KSA - Arábia Saudita
MEX - México
POL - Polônia
FRA - França
DEN - Dinamarca
TUN - Tunísia
AUS - Austrália
ESP - Espanha
GER - Alemanha
JPN - Japão
CRC - Costa Rica
BEL - Bélgica
CAN - Canadá
MAR - Marrocos
CRO - Croácia
BRA - Brasil
SRB - Sérvia
SUI - Suíça
CMR - Camarões
POR - Portugal
GHA - Gana
URU - Uruguai
KOR - Coréia do Sul

\*\* Como resposta dos exercícios podem ser inseridos os respectivos comandos SQL usados para resolvê-lo, ou referenciar um arquivo no GitHub.

### [M02S05] Ex 02 - Copa do Mundo (parte 2) - Consulta de Times

Realizar consultas na tabela de times:
a) Consultar o nome da seleção cuja sigla é 'KSA'.
b) Consultar a sigla da seleção de Gana.

\*\* Como resposta dos exercícios podem ser inseridos os respectivos comandos SQL usados para resolvê-lo, ou referenciar um arquivo no GitHub.

### [M02S05] Ex 03 - Copa do Mundo (parte 3) - Novas Consulta de Times

Realizar consultas na tabela de times:
a) Consultar todos os campos dos times cujo nome começa com 'E'.
b) Consultar os campos dos times que começam com 'E' e cuja sigla começa com 'U'.

### [M02S05] Ex 04 - Copa do Mundo (parte 4) - Novo campo de Grupos

Os times são organizados em grupos para jogarem entre si, cujos primeiros colocados passam de fase.

a) Alterar a tabela de TIMES, adicionando a coluna de 'grupo' (varchar).
b) Atualizar cada registro com o respectivo grupo em que faz parte, conforme listagem abaixo.
c) Consultar todos os times para conferir.

## GRUPO - TIMES

A - Qatar, Equador, Senegal, Holanda
B - Inglaterra, Irã, Estados Unidos, País de Gales
C - Argentina, Arábia Saudita, México, Polônia
D - França, Dinamarca, Tunísia, Austrália
E - Espanha, Alemanha, Japão, Costa Rica
F - Bélgica, Canadá, Marrocos, Croácia
G - Brasil, Sérvia, Suiça, Camarões
H - Portugal, Gana, Uruguai, Coréia do Sul

### [M02S05] Ex 05 - Copa do Mundo (parte 5) - Consultas de Times e Grupos

Realizar consultas na tabela de times:
a) Consultar o nome dos times do grupo G.
b) Consultar as siglas dos times do grupo C.

### [M02S05] Ex 06 - Copa do Mundo (parte 6) - Novas Consultas de Times e Grupos

Realizar consultas na tabela de times:
a) Consultar todos os campos dos times do grupo 'E' e do grupo 'H', em ordem alfabética de grupo.
b) Consultar todos os campos dos times do grupo 'E' e do grupo 'H', em ordem alfabética de nome do time.

### [M02S05] Ex 07 - Copa do Mundo (parte 7) - Tabela de Títulos da Copa

Cada seleção de futebol de cada país tenta acumular mais títulos que as demais.
Vamos armazenar os anos em que cada time que está participando da Copa atual ganhou alguma copa do mundo.

a) Criar a tabela CAMPEOES com os campos ano (int e primary key) e sigla_time (foreign key da tab de times).
b) Popular esta tabela com os dados listados abaixo.
c) Consultar os dados desta tabela para conferência.

## ANO - TIME CAMPEÃO (inserir a respectiva sigla no campo da tabela)

1930 - Uruguai
1950 - Uruguai
1954 - Alemanha
1958 - Brasil
1962 - Brasil
1966 - Inglaterra
1970 - Brasil
1974 - Alemanha
1978 - Argentina
1986 - Argentina
1990 - Alemanha
1994 - Brasil
1998 - França
2002 - Brasil
2010 - Espanha
2014 - Alemanha
2018 - França

### [M02S05] Ex 08 - Copa do Mundo (parte 8) - Consultas de Campeões

Realizar consultas na tabela de Campeões:

a) Consultar os campos da tabela de campeões ordenados pelo ano.
b) Consultar sigla do time campeão no último ano em que a copa foi disputada (dica: usar MAX).
c) Consultar a quantidade de títulos por sigla de time, ordenando da maior pra menor quantidade (dica: usar group by, count e order by).

### [M02S05] Ex 09 - Copa do Mundo (parte 9) - Novas Consultas de Times e Grupos

Realizar consultas na tabela de times:
a) Consultar os grupos cadastrados/existentes, sem repetir os grupos e em ordem alfabética (dica: usar distinct).
b) Consultar a quantidade de times em cada grupo (dica: usar group by).

### [M02S05] Ex 10 - Copa do Mundo (parte 10) - Novas Consultas de Times e Campeões

Realizar consultas na tabela de times e campeões:
a) Consultar os nomes em maiúsculo dos times que estão dispuntando a copa atual é que já ganharam algum título de campeão da Copa do Mundo, sem repetir o nome do time (dica: usar JOIN e DISTINCT)
b) Consultar os nomes em minúsculo dos times que estão dispuntando a copa atual é que nunca ganharam um título de campeão da Copa do Mundo, sem repetir o nome do time (dica: usar JOIN e DISTINCT)
