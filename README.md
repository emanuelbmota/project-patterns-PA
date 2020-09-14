# Padrão de projeto

## Pattern Name and Classification
  ###### Composite
  - É um padrão estrutural.
## Intent
 Modificar a estrutura de um objeto.
## Motivition
  Permite tratar nós folha e composição de maneira uniforme.
  - Exemplos:
    - Aplicação possui estrutura hierárquica e requer funcionalidades genéricas por toda a estrutura

    - Aplicação precisa agregar dados por toda a hierarquia

    - Aplicação precisa tratar composição e objetos individuais de maneira uniforme
    
## Applicability
  Aplicável para casos que requerem objetos que se comportam como estrutura em árvore para representar hierarquias todo-parte:
  - Cada nó (exceto raiz) é um composite ou nó folha.
## Structure  
  A estrutura é basicamente uma classe onde sua interface junto com seus elemntos e sub-elementos são relacionados entre si, como se fossem uma árvore. 
  
  Exemplo:
   - A classe 'Client' tem uma interface 'Component' onde ela descreve operações que são comuns tanto para elementos simples como para elementos complexos da árvore. Abaixo da interface temos um elemento 'Leaf (folha)' que não tem sub-elementos e executa alguma atividade, ao lado dele temos o elemento 'Composite' que tem seus sub-elementos onde ele delega suas atividades para seus childrens (filhos) e assim que os childrens terminam a atividade, eles retornam o valor para o 'Composite', assim devolvendo para o 'Component' e depois ao 'Client'.
## Participants
 ###### Component:
  - Declara interface para objetos da composição
  - Implementa comportamentos padrão comuns para todas as classes
  - Declara uma interface para acessar e gerenciar componentes filho

###### Leaf: 
  - Representa objetos folha da consição que não tem filhos
  - Define o comportamento para objetos primitivos da composição

###### Composite: 
  - Define o compotamento para componentes que possuem filhos
  - Armazena componentes filhos 
  - Implementa operações relacionadas a filhos e definidas na interface Component

###### Client:
  - Manipula os objetos da composição via interface Component


###### Sample Code
  ###### - Pastas no repositório
