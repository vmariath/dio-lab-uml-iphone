
# Título do Projeto

O seguinte projeto foi realizado para finalização da Trilha de Java POO realizada durante Bootcamp Claro DIO.

## Desafio

O desafio consiste modelar e diagramar uma representação UML de um componente iPhone, abrangendo suas seguintes funcionalidades

- Reprodutor Musical
- Aparelho Telefônico
- Navegador de Internet

Juntamente com a modelagem do diagrama UML, foi implementado as classes e interfaces correspondentes em Java.


# Diagrama UML

```mermaid
classDiagram
    class Iphone {
        +void tocar()
        +void pausar()
        +void selecionarMusica(String musica)
        +void ligar(String numero)
        +void atender()
        +void iniciarCorreioVoz()
        +void exibirPagina(String url)
        +void adicionarNovaAba()
        +void atualizarPagina()
    }

    class ReprodutorMusical {
        +void tocar()
        +void pausar()
        +void selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +void ligar(String numero)
        +void atender()
        +void iniciarCorreioVoz()
    }

    class NavegadorNaInternet {
        +void exibirPagina(String url)
        +void adicionarNovaAba()
        +void atualizarPagina()
    }

    Iphone ..|> ReprodutorMusical
    Iphone ..|> AparelhoTelefonico
    Iphone ..|> NavegadorNaInternet
