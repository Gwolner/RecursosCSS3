# CSS3 practice

Práticas de CSS para aperfeiçoar os conhecimentos já adquiridos

## Cronograma de práticas

* Sintaxe 
```css
seletor{
  propriedade:valor;
}
```

* Seletores universal, de tipo e de atributo
```css
/*Seletor universal. Comumente usado para definir o comportamento inicial de página.*/
*{
  margin: 0;
  padding: 0;
  color: red;
}
```

```css
/*Seletor de tipo.*/
h1{
  font-size: 40px;
  font-family: tahoma;
}

p{
  color: blue;
  font-size: 15px;
}
```

```css
/*Seletor de atributos.*/
input[type="submit"]{
  width: 200px;
  height: 25px;
  background-color: #ccc;
}

input[name="email"]{
  width: 200px;
  height: 25px;
  background-color: #ccc;
}
```

* Agrupamento de seletores
```css
h2, h3, p{
  color: red;
  text-align: center;
}
```

* Seletores id e class
```css
/*Seletor id.*/
#seletor-id{
  color: blue;
}
```

```css
/*Seletor classe.*/
.seletor-classe{
  color: gray;
}
```

* Dimensões (referência, width, height, min e max)
```css
/* Usado como referência para que o height possa utilizar outras unidades(em, vh, wh, em) além do px.*/
html,body{
  height:100%;
}
```
```css
  /*Largura*/
  width: 80%; /*Sem height a altura fica automatica, de acordo com o conteúdo.*/
  max-width: 800px; /*Define um tamanho máximo.*/
  min-width: 500px; /*Define um tamanho mínimo.*/  
```
```css
  /*Altura*/
  height: 50px; /*Sem width a largura ocupa 100% da tela.*/
  min-height:10px; /* Altura mínima desejada.*/
  max-height: 50px; /* Altura máxima permitida.*/
```

* Padding e Margin
```css
  /*Quatro lados iguais.*/
  
  padding: 20px;
  
  margin: 20px;
```

```css
  /*Quatro lados diferentes: sentido horário.*/
  
  padding: 10px 20px 30px 30px;
  
  margin: 10px 20px 30px 30px;
```

```css
  /*Declarações individuais dos lados.*/
  
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 30px;
  padding-left: 30px;
  
  margin-top: 20px;
  margin-right: 20px;
  margin-bottom: 20px;
  margin-left: 20px;
```

* Propriedades de texto
```css
  /*Posição do texto na página.*/
  text-align: left;
  text-align: center;
  text-align: right;
  text-align: justify;
```

```css
  /*Caixa alta e caixa baixa*/
  text-transform: capitalize; /*Apenas a primeira letra de cada palavra fica maíuscula.*/
  text-transform: lowercase;  /*Deixa todo o texto minúsculo.*/
  text-transform: uppercase; /*Deita todo o texto maiúsculo.*/
```

```css
  /*Traçar uma linha.*/
  text-decoration: line-through; /*Sobre o texto.*/
  text-decoration: overline;  /*Acima do texto.*/
  text-decoration: underline; /*Abaixo do texto.*/
```

```css
  /*Adiciona sombra ao texto.*/
  text-shadow: 3px 3px 4px #32CD32; /*X, Y, Desfoque (opcional), Cor da sombra.*/
  text-shadow: 4px 4px #32CD32; /*X, Y, Cor da sombra.*/
```

```css
  text-indent: 20px; /*Define um recuo na linha (uma espécie de parágrafo).*/
  
  line-height: 30px; /*Define a altura das linhas.*/
  
  direction: ltr; /*Direção de formação do texto: ltr ou rtl. O padrão é ltr (left to right).*/
  
  letter-spacing: 3px; /*Espaçamento entre as letras.*/
  
  word-spacing: 10px; /*Espaçamento entre as palavras.*/
```

* Box sizing e box shadow
```css  
  box-sizing: border-box; /*Mantem o tamanho definido da DIV, não somando com o padding.*/
  
  /*OBS: Recomenda-se usar em um seletor universal e não diretamente no elemento.*/
  *{
    box-sizing: border-box;
  }
```

```css
  box-shadow: 10px 10px 5px #A0522D; /*Atribui sombra ao elemento. Similar a atribuição para texto.*/
```

* Overflow e Opacity
```css

```
* Border radius
```css

```
* Fonts
```css

```

* @Font Face com [Font Squirrel](https://www.fontsquirrel.com/)
```css

```

* Font externa com [Google Font](https://fonts.google.com/)
```css

```

* Colors e Gradients
```css

```

* Float
```css

```

* Position
```css

```

* Border e Outline
```css

```

* Transition
```css

```

* Background
```css

```

