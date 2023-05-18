# Frandes-Bancarias

# Projeto 1 – Exploração e eliminação de dados espúrios
-------------------------

Este projeto tem a finalidade de desenvolver um modelo para prever, a partir de dados demograficos e históricos, se uma conta bancária pagara a sua dívida de crédito no próximo mês. A complexidade das tarefas aumentará conforme avançamos pelo curso; este projeto inicial envolvera: 

+ Realizar operacões básicas em Python.
+ Descrever o contexto do estudo de caso.
+ Executar operações que garantam a integridade dos dados. 
+ Fornecer resumos estatísticos e visualizar os dados do estudo de caso.
+ Implementar *one-hot-enconding* em variáveis indicadoras. 

## O problema:

Nosso cliente é uma companhia de cartão de crédito. Forneceram-nos uma base de dados que contém dados demográfico e financeiros (dos últimos seis meses) relacionados a uma amostra de 30.000 contas. Os dados estao organizados da seguinte forma: cada linha corresponde a uma linha de crédito, e as colunas guardam características relevantes a respeito dela. As linhas são rotuladas de acordo com a informação se após um período de seis meses o dono de determinada conta cumpriu com o pagamento mínimo.

## Objetivo:

O objetivo será desenvolver um modelo preditivo capaz de inferir se uma conta pagará ou não sua dívida no próximo mês, baseando-se nos dados históricos e demográficos fornecidos pelo cliente.

## Descrição dos Dados:

Os dados encontram-se no arquivo credito_clientes.csv, e suas colunas guardam as seguintes informações: 

+ LIMIT BAL: Limite de crédito fornecido pela empresa. 
+ EDUCATION: Nível escolar (1 = pos-graduação; 2 = curso superior; 3 = ensino médio; 4 = outros)
+ MARRIAGE: Estado civil (1 = casado; 2 = solteiro; 3 = outros)
+ AGE: Idade (anos)
+ PAY 1 - PAY 6: Historico de pagamentos anteriores, referentes aos meses de Abril a Setembro. 
    PAY 1 representa a situação do pagamento em Setembro; PAY 2 o pagamento em Agosto, e assim por diante até PAY 6, referente a Abril.
    Os valores das medidas significam: −1 = pagamento no prazo; 1 = pagamento atrasado em um mes; 2 = atrasado em dois meses, e assim por diante.
+ BILL AMT1 - BILL AMT6: Faturas do cartao de crédito.
+ PAY AMT1 - PAY AMT6: Quantia paga da fatura.
+ default payment next month: Se ele pagou ou não a fatura.
