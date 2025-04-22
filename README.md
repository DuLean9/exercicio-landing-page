# Projeto exercicio Landing Page
Um projeto para pratica com css e html 🚀

## Preview 📷

- Modelo realizado:

1 - Desktop

[<img src="./src/images/Animação-desktop.gif">]

2 - Mobile

[<img src="./src/images/Animação-mobile.gif">]

## Funcionalidades ⚙️
✔️ - O site tem como objetivo imitar uma landing page de uma agencia de viagens com um menu "hamburguer" no mobile

## Tecnologias utilizadas 👨‍💻
- HTML
- CSS

## Aprendizado 📖
```css 
body {
    display: grid;
    grid-template-areas: "header header header header"
                         "hero hero hero hero"
                         "about about about about"
                         "services services services services"
                         "projects projects projects projects"
                         "footer footer footer footer";
    grid-template-columns: repeat(4, 1fr);
}
```
```css
Exemplo
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr; /* 3 colunas */
  grid-template-rows: 100px 200px 100px; /* 3 linhas */
  grid-template-areas:  >>> posso usar só grid:
    "header header header" 50px para definir o tamanho da altura
    "sidebar content content" 300px
    "footer footer footer" 50px / 80px auto 80px; para definir a largura
}

.header {
  grid-area: header;
}

.sidebar {
  grid-area: sidebar;
}

.content {
  grid-area: content;
}

.footer {
  grid-area: footer;
}


```
- Utilizei a propriedade Display grid, grid-template-areas e grid-template-columns para a disposição dos meus elementos em tela.

  Logo apos, eu utilizei a propriedade gride-area para referir ao nome da classe dada ou meu elemento. 

- No modo responsivo, fiz a utilização do menu "hamburguer" somente com o CSS puro, com o uso do before e after e a propriedade transform

```css
.hero:after {
    content: url('../images/seta_preta.png');
    position: absolute;
    bottom: 40px;
    height: 35px;
    animation: arrow 0.6s infinite alternate ease-in-out;
}

@-webkit-keyframes arrow {
    0% {
        opacity: 0.5;
        transform: translateY(0);
    }
    100% {
        opacity: 0.9;
        transform: translateY(0.4em);
    }
}
```
- Utilizei o @-webkit-keyframes para fazer a animação de uma flecha (webkit para nevegadores mais antigos) e utilizei a propriedade animation para dar nome e valores a animação.

```css
:nth-child(n)
```
Utilizei o :nth-child(n) que é uma pseudo-classe em CSS que seleciona o enésimo filho de um elemento pai, com base na posição.

## Demonstração 👁️
🔗 Acesse o projeto aqui: (https://dulean9.github.io/exercicio-landing-page/)