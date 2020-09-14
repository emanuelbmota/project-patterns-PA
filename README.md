# Padrão de projeto

## Pattern Name and Classification
  Composite
  - É um padrão estrutural.
## Intent
 Modifica a estrutura de um objeto.
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
  A estrutura é uma basicamente uma árvore, onde temos uma classe que todos os elementos e sub-elementos são relacionados com ela.
  
  A estrutura é bascimente uma classe onde seus sub-elementos são relacionados entre si, como se fossem uma árvore. Exemplo:
   - A classe 'Client' tem uma interface 'Component' que descreve operações que descreve operações que são comuns tanto para elementos simples como para elementos complexos da árvore. Abaixo da interface temos um elemento 'Leaf (folha)' que não tem sub-elementos que faz alguma atividade e ao lado dele temos o elemento 'Composite' que tem seus sub-elementos onde ele delega suas atividades para seus childrens (filhos) e assim que os childrens terminam a atividade, eles retornam o valor para o 'Composite'.
## Participants
 ### Component:
  - Declara interface para objetos da composição
  - Implementa comportamentos padrão comuns para todas as classes
  - Declara uma interface para acessar e gerenciar componentes filho

### Leaf: 
  - Representa objetos folha da consição que não tem filhos
  - Define o comportamento para objetos primitivos da composição

### Composite: 
  - Define o compotamento para componentes que possuem filhos
  - Armazena componentes filhos 
  - Implementa operações relacionadas a filhos e definidas na interface Component

### Client:
  - Manipula os objetos da composição via interface Component


## Sample Code
  https://repl.it/@JoaoRonaldo/CompositePattern#Main.java
