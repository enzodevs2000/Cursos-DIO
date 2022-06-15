# Introdução ao FlexBox

## Estrutura de Container

Temos um elemento pai que assume o comportamento de um **Flex Container** e, este pode ter filhos que são os **Flex Items**

## Flex Container

### Propriedades relacionadas:

* display -> iniciador do container
* flex-direction -> faz o direcionamento dos itens
* flex-wrap -> Se aplica para quebra ou não de linha
* flex-flow -> abreviação do direction e do wrap
* justify-content -> Alinha os itens do container de acordo com a usa direção
* align-items -> alinha os itens de acordo com o seu eixo do container 
* align-content -> alinha as linhas do container.

## Flex Items

São filhos diretos do Flex Container. Mas, também, pode ser Flex Container se a propriedade **display** for aplicada e ter seus próprios itens, ou seja, **Flex Items**.

### Propriedades relacionadas:

* flex-grow -> definer o fator de crescimento
* flex-basis -> define o tamanho inicial do item
* flex-shrink -> define a capacidade de redução
* flex -> abreviação para as 3 propriedades anteriores
* order -> Relaciona a ordem de distribuição
* align-self -> Define o alinhamento para um item específico do container

