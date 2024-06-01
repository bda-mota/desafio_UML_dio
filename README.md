# desafio_UML_dio
modelar e diagramar a representação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.

## Funcionalidades a Modelar
Reprodutor Musical
Métodos: tocar(), pausar(), selecionarMusica(String musica)
Aparelho Telefônico
Métodos: ligar(String numero), atender(), iniciarCorreioVoz()
Navegador na Internet
Métodos: exibirPagina(String url), adicionarNovaAba(), atualizarPagina()

## Diagrama UML

![UML](https://github.com/bda-mota/desafio_UML_dio/raw/main/uml_dio.png)

```mermaid
classDiagram
    class iPhone {
        - modelo: String
        + ReprodutorMusical()
        + AparelhoTelefonico()
        + NavegadorInternet()
    }

    class ReprodutorMusical {
        + tocar(): void
        + pausar(): void
        + selecionarMusica(musica: String): void
    }

    class AparelhoTelefonico {
        + ligar(numero: String): void
        + atender(): void
        + iniciarCorreioVoz(): void
    }

    class NavegadorInternet {
        + exibirPagina(url: String): void
        + adicionarNovaAba(): void
        + atualizarPagina(): void
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
``` 
