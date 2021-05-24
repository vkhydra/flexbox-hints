# Flexbox

Informações com referências de cursos da [Alura](https://cursos.alura.com.br) e de um projeto feito na ORIGAMID, o qual não sou autor. As refências do mesmo e outras informações podem ser encontradas no rodapé próprio site.

[Link do projeto](https://origamid.com/projetos/flexbox-guia-completo/)

# Como usar o Flexbox

## 1° - Pergunte às tags, ou classes...

Pergunte para as tags, ou classes, quem é o pai. A tag/classe pai deverá receber no CSS o seguinte parâmetro:

```css
classe-pai {
  display: flex;
}
```

> Obs.: Classes filhos ficarão com tamanhos iguais caso o pai receba display flex.

## 2° - Alinhar itens ao centro da classe pai...

Para esta ação, devemos apenas adicionar o seguinte parâmetro a classe pai:

```css
classe-pai {
    ...
  align-items: centro;
}
```

## 3° - Distribuir espaço igual entre os elementos...

Nesse caso, precisamos ter um espaço em restante no espaço pai.
Por exemplo:

![Barra de navegação com título "Alurinha" à esquerda e um menu à direita.](./img/3-space-between.jpeg)

Utilizaremos o parâmetro:

```css
classe-pai {
    ...
  justify-content: space-between;
}
```

O resultado será:

![Barra de navegação com título "Alurinha" à esquerda, menu ao meio, e um espaço à direita.](./img/3-space-between-fixed.jpeg)

## 4° - Distribuir espaço equivalente entre os elementos...

Para isso, utilizaremos um parâmetro parecido com o anterior:

```css
classe-pai {
    ...
  justify-content: space-around;
}
```

![Exemplos de espaços com between e around.](./img/4-around.jpeg)

## 5° - Organizar itens em colunas...

Lembrando que para utilizar comandos flex, precisamos que a classe pai, referente ao filho que estamos trabalhando, receba <code>display: flex;</code>. Com isso feito, utilizaremos <code>flex-direction</code>, o qual define a direção dos itens. Para esse caso utilizaremos a propriedade <code>column</code>. Ela separa cada item do pai em colunas.

**_Obs:_** Por padrão de sistema, o <code>flex-direction</code> tem como parâmetro <code>row</code>, ou seja, em linha.

![Exemlplo da utilização de column](./img/column.jpeg)

## 6° Quebrar linhas...

Para isso, utilizaremos o comando <code>flex-wrap</code>. Esse comando poderá receber 3 parâmetros:

```css
 {
  flex-wrap: nowrap;
  flex-wrap: wrap;
  flex-wrap: wrap-reverse;
}
```

Lembrando que é recomendável que o elemento pai tenha um valor de altura.

![Exemplo da utilização de flex-wrap](./img/wrap.jpeg)

## 7° O flex-flow é um atalho bem útil...

Para usar <code>flex-direction</code> e <code>flex-wrap</code> de uma vez só podemos utilizar o <code>flex-flow</code>. Ele recebe dois parâmetros, o primeiro indicará se é uma coluna ou uma linha, o segundo se é um quebra linha ou não:

```css
 {
  flex-flow: [row/column] [wrap/nowrap];
}
```
