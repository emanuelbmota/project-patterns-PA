# Padrão de projeto

## Pattern Name and Classification
  ###### Template Method
  - É um padrão comportamental.
## Intent
  Define um esqueleto de um algoritmo na superclasse mas deixa as subclasses sobrescreverem etapas específicas do algoritmo sem modificar sua estrutura.

## Motivition
  - Aplicação possui estrutura hierárquica e um algoritmo que pode ser dividido em etapas.
  - Dois ou mais componentes diferentes implementam esse algoritmo, possuindo várias semelhanças mas algumas diferenças na implementação de algumas etapas do algoritmo.
  - Alterações no algoritmo pode ser feitas de forma genérica ou específica em cada componente específico.
  - Útil em cenários em que se tem gerador automático de código.
    
## Applicability
  Aplicável para casos em que se tem uma hierarquia de classes se tem um algoritmo que deve ser dividido em etapas.
  - Exemplos:
    - Um método na superclasse, chamado template method, invoca os demais métodos que podem ser abstratos.

## Structure  
  Formada de uma 'Classe Abstrata' e uma 'Classe Concreta'.
  
  - Classe Abstrata:
    A Classe Abstrata declara método que agem como etapas de um algoritmo, bem como o próprio método padrão que chama esses métodos em uma ordem específica. Os passos podem ser declarados como abstratos ou ter alguma implementação padrão.

  - Classe Concreta:
    As Classes Concretas podem sobrescrever todas as etapas, mas não o próprio método padrão.

## Participants
 ###### FrameworkClass:
  - Define o templateMethod que é responsável por chamar os demais métodos.
  - Especifica os métodos abstratos das etapas de execução.

###### ApplicationClassOne/ApplicationClassTwo: 
  - Redefine, quando necessário, algumas etapas do algoritmo especificado em FrameworkClass.
  
###### Sample Code
  ###### - Pastas no repositório
