# MonitoramentodeEstruturas
Esse programa utiliza o python para otimizar o acompanhamento de operações estruturadas feitas com derivativos
Primeiro é definida a função para utilizar o black and scholes.
depois é feito a importação das estruturas com quantidade, valor recebido na operação a crédito e o Ticker dos derivativos envolvidos.
Juntamente com a grade de opções em aberto na B3
Depois o programa fará um join entre esses dois DataFrames por meio do ticker da opção, identificando o ativo subjacente, vencimento e Strike.
Feito isso, por meio da API do yahoo finance, o programa pegará o preço atual dos ativos subjacentes, e pela API do workalendar fará a conta de quantos dias úteis faltam até o vencimento daquele derivativo, e importará a vol implícita de 30 dias atual dos ativos subjacentes.
Depois aplicará a Fórmula de B&S para todos os ativos e então saberá quanto e se uma operação está dando lucro ou prejuízo, e qual é sua situação.
Por último por meio de um bubble graph, fará um mapeamento das operações em relação ao lucro.
