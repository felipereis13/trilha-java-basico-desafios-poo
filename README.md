# trilha-java-basico-desafios-poo
Segue diagrama UML do desario poo:

```mermaid

classDiagram 

    Iphone <|-- aparelhoTelefone
    Iphone <|-- reprodutorMusical
    Iphone <|-- navegadorInternet
    aparelhoTelefone <|-- smartphone
    reprodutorMusical <|-- ipod
    navegadorInternet <|-- safari
    class aparelhoTelefone {
        <<interface>>
      +ligar(String numero)void
      +atender()void
      +inciarCorreioVoz()void
    }
    class reprodutorMusical{
        <<interface>>
      +selecionarMusica()void
      +tocar()void
      +pausar()void
    }
    class navegadorInternet{
        <<interface>>
      +exibirPagina(String url)void
      +adicionarNovaAba()void
      +atualizarPagina()void
    }
    
    
    
