# CSS3 practice

> Práticas de CSS para aperfeiçoar os conhecimentos já adquiridos, além de servir como consulta aos devs que estão iniciando no mundo das folhas de estilo em cascata.

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
  /*Overflow - Trata do excedente de texto de um elemento.*/
  
  overflow: auto; /*Adiciona barra apenas quando e onde for necessária.*/
  overflow: visible; /*Default. Texto excede normalmente o elemento.*/, 
  overflow: hidden; /*Oculta o texto excedente.*/
  overflow: scroll; /*Cria uma barra de rolagem*/
  
  /*Opacity*/
  
  opacity: 0.3; /*Os valores variam de 0 (0%) até 1 (100%)*/
```

* Border radius
```css
  border-radius: 20px; /*Cria todos os vértices arredondados.*/
  
  border-radius: 20px 50px; /*Cria vértices arredondados de formas opostas.*/
  
  border-radius: 20px 50px 100px; /*Cria três vértices arredondados, sendo o quarto igual ao segundo.*/
  
  border-radius: 20px 50px 100px 200px; /*Quatro vértices distintos.*/
  
  /*Altera os vértices individualmente.*/
  border-top-left-radius: 20px;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 50px;
  border-bottom-left-radius: 35px;
```

* Fonts
```css
  font-family: Arial, "Times New Roman", serif; /*Define famílias de fontes que podem ser usadas.*/
  font-variant: small-caps; /*Os valores possíveis são small-caps e normal (default)*/
  font-weight: bold; /*Os valores possíveis são bold (negrito) e normal (default) */
  font-style: oblique; /*Os valores possíveis são italic, oblique (um italico mais inclinado) e normal (default)*/
  font-size: 2.5em; /*2.5em equivale a 4px.*/
  
  /*OBS: A unidade "em" é usada para questões de acessibilidade, usando o referencial *{font-size: 100%;}.
  
  Ex: 40px (valor desejado) / 16 (contexto de unidade relativa) = 2.5em.*/
```

* @Font Face com [Font Squirrel](https://www.fontsquirrel.com/)
```css
  /* Importando um arquivo de fonte */
  @font-face{
    font-family: alexbrush-regular-webfont;
    src: url(../alexbrush-regular-webfont.woff);
  }
  
  /*Usando arquivo importado*/
  font-family: alexbrush-regular-webfont;
  font-size: 2.5em;
```

* Font externa com [Google Font](https://fonts.google.com/)
```html
  <!-- Copiar e colar o link diretamente do Google fonts -->

  <link href="https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap" rel="stylesheet"> 
```

```css
  font-family: "Indie Flower", cursive;
  font-size: 2.5em;
```

* Colors e Gradients
```css
  /*Colors*/




  /*Gradients*/
  background: linear-gradient(red, green); /*Duas cores.*/
  
  background: linear-gradient(to right, green, blue); /*Duas cores seguindo pra direita.*/

  background: linear-gradient(to top, green, red, blue); /*Três cores seguindo pra cima.*/

  background: linear-gradient(to top left, red, green); /*Duas cores seguindo pra cima e esquerda.*/

  background: linear-gradient(50deg, orange, blue, red); /*Três cores com 50 graus de inclinação */
  
  background: linear-gradient(rgba(255,0,0,0.8), red, blue); /*Usando RGB ou RGBA.*/
  
  background: radial-gradient(orange, blue); /*A origem é sempre o centro.*/
```

* Float
```css
  float:left;
  
  float: right;
```

* Position
```css
  position: absolute;  /*Usa um referencial: a página ou um "position: relative".*/

  position: relative; /*Tira a referência da página e atribui a este elemento.*/
  
  /*Outros valores para position são: static (default) e fixed (deixa o elemento fixo na tela e não na página).*/
```

* Border e Outline
```css
  /*Border*/
  
  border-style: dotted; /*Estilo da borda. dashed, solid, double, groove, ridge, inset, outset e dotted*/
  border-color: #FF7F50; /*Cor da borda.*/
  border-width: 5px; /*Tamanho da borda.*/
  
  border: outset 5px #DB7093; /*Definindo três propriedades da borda (estilo, tamanho e cor).*/
  
  /*Definindo apenas uma borda.*/
  border-top: double 5px #BA55D3; /*Definindo apenas a borda superior*/
  border-right: dotted 5px #DB7093; /*Definindo apenas a borda direita*/
  border-bottom: dashed 5px #DB7093; /*Definindo apenas a borda inferior*/
  border-left: solid 5px #4B0082; /*Definindo apenas a borda esquerda*/
  
  /*Outline*/
  
  outline-style: ridge; /*Estilo do contorno (borda da borda).*/
  
  outline-width: 5px; /*Tamanho do contorno.*/
  
  outline: dotted 5px #FF0000; /*Definindo três propriedades do contorno (estilo, tamanho e cor).*/
  
  outline-offset: 15px; /*Distancia entre a borda e o contorno.*/

```

* Transition
```css
  /*Transição*/
  transition-property: width;
  transition-duration: 2s;
  transition-timefunction: linear;
  transition-delay: 2s;

  /*Propriedade estenográfica.*/
  transition:width 2s linear 1s;
  
  /*Mais de uma propriedade estenográfica.*/
  transition:width 2s linear 1s, height 2s linear 1s;
	
  transition:all 2s linear; /*Sem delay para que a animação seja imediata.*/
```

* Background
```css
  background-image:url(../img/fundo.jpg); /*Adiciona imagem.*/
  
  /*Repetição de imagem*/
  background-repeat: repeat-x; /*Repete imgaem apenas na horizontal.*/
  background-repeat: repeat-y; /*Repete imgaem apenas na vertical.*/
  background-repeat: no-repeat; /*Repete imgaem apenas na horizontal.*/
  
  background-position: 300px 500px; /*Coordenadas para posicionamento do background.*/

  /*Coordenadas predefinidas.*/
  background-position: left;
  background-position: center;
  background-position: right;
  
  background-position: right bottom;
  background-position: left top;

  /*Fixar background*/
  background-attachment:fixed; /*Valor padrão é scroll.*/
  
  /*Definindo o tamanho.*/
  background-size: 300px 500px;
  background-size: 100% 100%;
  
  /*Propriedade estenografica*/
  background: url(../img/fundo.jpg) center center 100% 100% no-repeat fixed;
```

