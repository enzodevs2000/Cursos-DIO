# Algumas estilizações no CSS

Modificamos a margin, padding, and border no css utilizando o próprio nome.

## margin, padding 
~~~css
    #exemplo {
        margin: 10px;
        margin: 10px 15px;
        margin: 10px 15px 20px 25px;

    }
~~~

No exemplo acima vemos 3 formas de definirmos a margem do elemento. Na primeira, definimos o valor da margem para todos os lados do elemento. Na segunda, o primeiro valor define a margem do eixo y e a segunda do eixo x. Por fim, a terceira define o valor para a seguinte ordem: top, right, bottom, left. 

A mesma ideia serve para o *padding*.

Outra forma de definir esses valores é usando as propriedades específicas:

* `margin-top:`
* `margin-right:`
* `margin-bottom:`
* `margin-left:`

## background

A background é um atributo que define o fundo dos elementos. Algumas variações do *background*:

* `background-color:`
* `background-image: url(caminho-arquivo)`
* `background-position:`

### background-color
Temos 3 formas de definirmos a cor:

* nome da cor em inglês
* valor em hexa
* valor em rgb

## border

O atributo border segue a seguinte estrutura:

~~~css
    #exemplo {
        border: 1px solid #b2d4c3
    }
~~~

o primeiro valor representa o tamanho da borda, o segundo o tipo da borda e o terceiro a cor. Assim como a margin e o padding, podemos definir os valores específicos para cada lado.

Ainda podemos também definir cada um dos valores de forma específica:

* `border-width: 1px`
* `border-style: dotted/dashed/solid`
* `border-color: cyan`

Temos também, o atributo `border-radius` que define curvatura para os cantos da borda.

**OBS**: o valor 50% faz o elemento ficar circular.

