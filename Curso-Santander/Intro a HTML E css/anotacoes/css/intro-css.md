# Introdução ao CSS 

O CSS é uma linguagem de estilização que complementa o HTML. Ele é formado pela seguinte estrutura:

~~~css
    p {
        color: #fff;
        font-size: 20px;
    }
~~~

*p* no exemplo acima é um seletor, no caso para a tag de parágrafo. Em seguida, abrimos chaves e entre elas colocamos as propriedades e sesus valores. No exemplo acima, estamos modificando a cor e o tamanho da fonte.

## Ids e Classes

No HTML podemos declarar ids e classes em nossas estruturas. Isso é muito útil, pois nos permite criar diferentes estilizações para cada um com o CSS.

A diferença entre o *Id* e a *class* é que o id é usado para representar uma estrutura única, enquanto que a classe é uma estilização que pode ser reutilizada.

Para estilizarmos um id devemos fazer como no exemplo:

~~~css
    #title {
        font-style: italic;
    }
~~~

Enquanto que classes é da seguinte forma:

~~~css
    .subtitle {
        margin: 10px;
    }
~~~

Para podermos usar o css no nosso arquivo html devemos importá-lo. Para isso, devemo utilizar a tag `<link rel="stylesheet" href="caminho-arquivo">` na `<head>` do html.