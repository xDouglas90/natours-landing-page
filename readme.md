<h1 align="center">Natours - Landing Page</h1>
<p align="center">Projeto feito em curso com objetivo de aprendizado em **CSS3** & **SASS**.</p>

<img src="https://img.shields.io/static/v1?label=build&message=HTML5&color=E34F26&style=for-the-badge&logo=html5"/>  <img src="https://img.shields.io/static/v1?label=build&message=css3&color=1572B6&style=for-the-badge&logo=css3"/> <img src="https://img.shields.io/static/v1?label=build&message=sass&color=CC6699&style=for-the-badge&logo=sass"/> <img src="https://img.shields.io/static/v1?label=deployed&message=vercel&color=000000&style=for-the-badge&logo=vercel"/>

------------

- Este projeto foi realizado sob tutoria de <a href="https://codingheroes.io/">Jonas Schmedtmann</a> no curso <a href="https://www.udemy.com/course/advanced-css-and-sass/">Master CSS and SASS</a>.
- Você pode visualizar o resultado do meu projeto <a href="https://natours-azure.vercel.app/">Clicando Aqui</a>.

------------
### Realizações

- A melhor maneira de realizar um reset básico no *CSS*, utilizando o seletor universal `*`:
```css
*,
*::after,
*::before {
  box-sizing: inherit;
  margin: 0;
  padding: 0;
}
```

- Como estruturar as definições de fonte para todo o projeto:
<img alt="Demonstração de código e estrutura para definições de fontes" title="Demonstração de código e estrutura para definições de fontes" src="https://images4.imagebam.com/14/ec/53/ME25JI3_o.png" height="200" />

#### - Header
- Como cortar partes de elementos utilizando `clip-path`:
```css
-webkit-clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
```
<img alt="Printscreen do resultado" title="Printscreen do resultado" src="https://images4.imagebam.com/42/c1/72/ME25JPI_o.png" height="250"/>

- A maneira mais fácil de centralizar elementos com as propriedades `top` e `left` do `transform`:
```css
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
```

- Como criar animações *CSS* utilizando `@keyframes` e a propriedade `animation`:
```scss
@mixin moveInX($direction, $initX, $midX, $finalX) {
  @keyframes moveIn#{$direction} {
    0% {
      opacity: 0;
      transform: translateX($initX);
    }

    80% {
      transform: translateX($midX);
    }

    100% {
      opacity: 1;
      transform: translateX($finalX);
    }
  }
}
```

```css
animation: moveInRight 1s ease-out;
```
<img alt="Gif do resultado" title="Gif do resultado" src="https://media.giphy.com/media/onegSI78u3s0U0TLzF/giphy.gif" />


