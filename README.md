# Desafio Semantix 

## Instalando pacotes necessários 

`` funcao_pacote = function(pacote){
if(!(pacote %in% installed.packages())){ 
  install.packages(pacote)
}
  library(pacote)
}
  
pacotesNecessarios = c('dplyr', 'ggplot2', 'party')

for(i in pacotesNecessarios){
  funcao_instala(pacote = i)
} ``


## Descrição do problema

+ Dados relacionados com campanha de marketing direto de uma instituição bancária. 
+ As campanhas de marketing foram baseadas em chamadas telefônicas.
+ Contatavam o cliente mais de uma vez para acessar se o produto (depósito a prazo bancário) seria aceito ou não.

## Variáveis

Input: 
  
  + Informações sobre o cliente
   
    1. idade (numérica)
    2. emprego: tipo de emprego
    3. estado civil (levando em consideração que "divorciado"" significa divorciado ou viúvo)
    4. educação
    5. tem crédito?
    6. saldo médio anual 
    7. tem empréstimo imobiliário? 
    8. tem empréstimo pessoal?
  
  + Informações sobre o último contato da campanha atual: 
   
    9. contato
    10. último dia de contato no mês
    11. mês do último contato do ano 
    12. duração do último contato em segundos
    13. número de contatos realizados durante esta campanha
    14. número de dias que passaram depois que o cliente foi contatado pela última vez de uma campanha anterior (-1 significa que o cliente não foi contatado anteriormente)
    15. número de contatos realizados antes desta campanha
    16. resultado da campanha de marketing anterior
    
Output: 
  
  + Variável de interesse: 
  
    17. o cliente assinou um depósito a prazo?
  

