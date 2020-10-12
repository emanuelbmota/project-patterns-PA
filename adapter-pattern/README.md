# Padrão de projeto

## Pattern Name and Classification
  ###### Composite
  - É um padrão estrutural.
## Intent
 A inteção para o uso do Adapter é fazer uma integração simples de dois códigos distintos em uma única aplicação.
## Motivition
  A motivação para o uso dessa tecnologia seria para faciliar o processo de integração de sistemas, poupando tempo e deixar os processos mais ágeis.
    
## Applicability
  A principal aplicação é quando temos que integrar dois sistemas diferentes, outra forma seria quando criamos um novo sistema e queremos integrar com uma API. Ele também é muito útil quando ja temos um sistema antigo e desatualizado, usando o adapter você vai conectando o sistema antigo de pouco em pouco até fazer a integração total.

## Structure  
  ![alt text](http://videos.web-03.net/artigos/Higor_Medeiros/PadraoAdapter_Java/PadraoAdapter_Java1.jpg) 
  
## Participants
 
 No diagrama de classe tem o Client, que é quem acessa a interface do Adaptador e a partir desta interface ele fará uma solicitação ao adaptador. O Adaptador, por sua vez, implementa a interface alvo (Target) e comunica-se com o Adaptee. O Adaptee é a nova biblioteca do fornecedor que está sendo inserida no sistema.


###### Sample Code
  ###### - Pastas no repositório
