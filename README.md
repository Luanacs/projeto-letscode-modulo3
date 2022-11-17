# Projeto Let's Code - Módulo 3 Técnicas de Programação I

## Projeto desenvolvido durante o terceiro módulo do curso de Data Science with Python da Let's Code from Ada em parceria com a Suzano.


#### Nesse projeto trabalharemos com dados fictícios de investidores.

<p> Serão 3 arquivos que devem ser carregados para responder as perguntas abaixo.

Informações

Cadastro:

id : Identificação do investidor
Nome : Nome completo do investidor
Sexo : Feminino ou masculino
Nasc : Data de nascimento
Idade : Idade do investidor
Email : E-mail do investidor
Lat_long : Dados geográficos do investidor
Job : Profisão do investidor ou do seu responsável (em inglês)
Estado : Estado onde o investidor reside
Investimento:

id : Identificação do investidor
Salario : Renda do investidor ou seu responsável
Perfil : Perfil de investimento
Ativo01, Ativo02, Ativo03, Ativo04, Ativo05, Ativo06, Ativo07 : O quanto de dinheiro o investidor colocou em cada ativo
Nota1, Nota2 : O quanto o investidor está satisfeito com nossa empresa (2 avaliações)
Lembrando que esses dados são irreais e fictícios

Arquivo cadastro.csv

Arquivo investimento.csv (dividido em 2 partes)

Critérios de avaliação
Os seguintes itens serão avaliados:

Reprodutibilidade do código: seu código será executado e precisa gerar os mesmos resultados apresentados por você;

Clareza: seu código precisa ser claro e deve existir uma linha de raciocínio direta. Comente o código em pontos que julgar necessário para o entendimento total;

Explicação de todos os processos feitos e decisões tomadas

Informações Gerais sobre o Projeto
O projeto poderá ser desenvolvido individualmente ou em grupos com até 4 pessoas, caos façam em grupos enviar a relação de alunos do grupo para o professor;
Data de Entrega: 18/11/2022;

Entrega: Através do Class

1 - Carregar os arquivos e cadastro, investimento1 e investimento2 e mostrar a quantidade de linhas de cada um, além das informações desses dataframes
[ ]
import pandas as pd
import datetime as dt

2 - Juntar os dataframes de investimento1 e investimento2 em um só e ver a quantidade de linhas
[ ]

3 - Crie um novo dataframe eliminando as linhas duplicadas
[ ]

4 - Junte o dataframe de investimento com o de cadastro
Dica: use a chave id

[ ]

5 - Ordene o dataframe pelo id, de forma crescente e redefina o índice
[ ]

6 - Faça uma análise dos dados faltantes e trate-os
Mostre todas as colunas com dados faltantes, sua quantidade/porcentagem e como tratar (preencher) cada uma delas explicando sua estratégia

[ ]

7 - Manipule os dados a seguir:
Criar coluna "Total" somando o valor de todos os ativos por investidor
Criar coluna "Media" com a média das notas 1 e 2
Criar coluna "Dominio" com apenas o domínio do email (dica: separar por @)
Mudar o nome da coluna "Salário" para "Renda" e tratar a coluna (sem caracter $ e tipo numérica)
Mudar os dados da coluna "Sexo" para Masculino e Feminino (tente usar o map)
Transformar os dados da coluna Media em inteiro
Criar coluna "NPS" onde o investidor é promotor se a média das notas é maior igual a 80, neutro se a média estiver entre 50 e 80, e detrator se for abaixo de 50
[ ]

8 - Calcule os seguintes dados
Calcule o total investido em cada coluna Ativo (tente usar o apply)
Qual o menor valor investido em cada ativo?
Mostre a média e desvio padrão de cada ativo
Qual a idade do investidor mais velho?
Qual a mediana da coluna Média?
[ ]

9 - Responder as perguntas abaixo
Quantos investidores são promotores?

Quantos investidores são do sexo feminino?

Quantos investidores investiram mais de 16000 no Ativo04?

Quantos investidores investiram mais de 16000 no Ativo04 e menos de 5000 no Ativo05?

Quantos investidores do sexo feminino tem mais de 25 anos e investiu menos de 10000? (bonus: por que esse dado seria importante para a estratégia da nossa empresa?

Quantos investidores tem em cada estado (dica: use groupby)

Qual é a soma do total investido por cada estado?

Como os investidores se distribuem em promotores, detratores e neutros?

Qual é a média do total investido por promotores, detratores e neutros? </p>
