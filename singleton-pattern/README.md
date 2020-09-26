# Padrão de projeto

## Pattern Name and Classification
  ###### Singleton
  - É um padrão criacional.
## Intent
  Define que uma, e somente uma instância concorrente de uma classe existirá no ciclo de vida da aplicação.

## Motivition
  - Quando houver a necessidade de acesso a um recurso a partir de uma instância.

  - Quando há uso em larga escala de um recurso em que se pode ter somente uma instância, reduzindo problemas de referência.
    
## Applicability
  Aplicável para casos em que se precisa controlar a forma como a classe é instanciada.

  - O construtor da classe é protegido
  - Todo o programa usa o Singleton para acessar os comportamentos nele definidos.

## Structure  
  
  - Classe Singleton:
    - É a única classe deste padrão.
    - O construtor é privado, não sendo acessível externamente.

  - Client:
    - É quem usa o Singleton.
    - Está interessado na instância, não importa se é uma só no programa todo.

## Participants

  
###### Sample Code
  ###### - Pastas no repositório
