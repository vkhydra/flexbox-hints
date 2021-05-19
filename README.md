# Flexbox



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