# Factory Method

o Factory Method é um padrão criacional que define uma interface para criar um objeto, mas deixa que as subclasses decidam qual classe instanciar.


# Intenção

Ele facilita quando a criação envolve uma serie de objetos (hierarquia). Facilita tambem pois disponibiliza um metodo que permite criar objetos, centralizando as dependencias em um unico ponto.

# Motivação

Quando se tem uma estrutura complexa de classes que demanda dependencia com varios tipos e quando se deseja reduzir o acoplamento entre as classes, com um unico ponto de responsabilidade.

# Aplicabildade

Podemos usar o factory method quando não sabemos de antemão os tipos e dependencias do objeto que o código deve trabalhar.


## Participante

![alt text](https://miro.medium.com/max/985/1*Fvyhz4KX0zSJB1ldvbnk3A.jpeg)

Client: É quem tem dependência com IProduct.

Creator: Define o Factory Method para retornar instância do ConcreteProduct.

IProduct: Define a interface de objetos que o factory cria.

ProductA:, ProductB: implementa a interface product.

## Estrutura

![alt text](https://miro.medium.com/max/985/1*Fvyhz4KX0zSJB1ldvbnk3A.jpeg)


# Exemplo:

Um exemplo a ser mostrado é um criado pelo professor. Se encontra na pasta Factory_Method/Exemplo.




