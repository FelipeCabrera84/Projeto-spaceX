Organização do projeto
1. Criar os 3 html (index.html, falcon9, humanFlight) | Criar pasta do Sass| Colocar pasta de imagens
2. Instalar o Bootstrap, tanto o CSS quanto script através do link https://getbootstrap.com/docs/5.1/getting-started/...
3. Colocar o title e o favicon do site
4. Fazer a criação do CSS através do Sass
sass --watch sass/style.scss:css/style.css
5. Linkar o CSS
6. Instalar a lib de animação de texto https://michalsnik.github.io/aos/

Home do projeto
1. Criar o primeiro container, que terá classe container00 e container01, para usarmos a herança do Sass( ela vai pegar a div do header e a div do primeiro texto.
<div class="container-fluid container00 container01">
         <div class="container">
         </div>
    </div>
2. Colocar depois disso o header dentro do segundo container, para criar a navbar
<header class="header">
<nav class="navbar navbar-expand-lg navbar-dark bg-transparent pt-4">
<div class="container-fluid">
<a class="navbar-brand" href="/index.html">
<img src="/imagens/logo-obc-2021-darkbg.png" alt="logoOneBitCode" class="logoPc">
</a>
<button class="navbar-toggler" type="button" data-bs-toggle="collapse"data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"aria-label="Toggle navigation">
<span class="navbar-toggler-icon"></span>
</button>
<div class="collapse navbar-collapse" id="navbarNav">
<ul class="navbar-nav">
<li class="nav-item">
<a class="nav-link active" aria-current="page" href="/falcon9.html">FALCON 9</a>
</li>
<li class="nav-item">
<a class="nav-link active" href="/humamFlight.html">HUMAN SPACE FLIGHT</a>
</li></ul>
</div>
</div>
</nav>
</header>
3. Colocar dentro de container01 uma div apenas para o título e para o botão
<div class="container titlePadding" data-aos="fade-up" data-aos-duration="1500">
            <p class="h5" id="lauchComing">LANÇAMENTO A CAMINHO</p>
            <p class="h1">MISSÃO EQUIPE-3</p>
            <button type="button" class="btn btn-outline-light mt-5" id="button">SAIBA MAIS</button>
            <div class="container text-center">
                <img src="/imagens/home/arrowDown.gif" alt="arrowDown" class="arrowDown">
            </div>
        </div>
4. Colocar agora, um novo container, com as mesmas características do de cima, mudando apenas a segunda classe
<div class="container-fluid container00 container02">
</div>
5. Dentro dela, vai vir uma outra div com o container de fato e outra classe chamada titlePadding
<div class="container titlePadding">
</div>
6. Agora sim vêm os títulos da página, colocando dois textos e 1 botão para o título
<p class="h5" id="lauchComing">MISSÃO CONCLUÍDA</p>
<p class="h1 shortTitle">MISSÃO EQUIPE-2 RETORNOU PARA A TERRA</p>
<button type="button" class="btn btn-outline-light mt-5" id="button">SAIBA MAIS</button>
7. Iremos para o container 03, basta copiar o container 02 e mudar os textos, dessa forma vamos ter uma economia de tempo.
<div class="container-fluid container00 container03">
         <div class="container titlePadding" data-aos="fade-down" data-aos-duration="1500">
            <p class="h5" id="lauchComing">MISSÃO CONCLUÍDA</p>
            <p class="h1 shortTitle">DRAGON RETORNOU PARA A TERRA</p>
            <button type="button" class="btn btn-outline-light mt-5" id="button">SAIBA MAIS</button>
        </div>
    </div>
8. Mesma coisa com o 4, que nesse caso é o último container da página
<div class="container-fluid container00 container04">
         <div class="container titlePadding" data-aos="fade-down-right" data-aos-duration="1500">
            <p class="h1 mediumTitle">STARSHIP POUSA ASTRONAUTAS DA NASA NA LUA</p>
            <button type="button" class="btn btn-outline-light mt-5" id="button">SAIBA MAIS</button>
        </div>
    </div>
9. Agora iremos para o footer. Faremos ele por sí só um footter, que terá um container fluid e uma classe chamada footer
<footer class="container-fluid footer">
</footer>
10. Agora colocaremos os elementos do footer, um span para ser o texto de copyright, e 3 âncoras para colocarmos
<span class="me-4 copyOBC">OneBitCode © 2021</span>
<a href="https://www.instagram.com/onebitcode/?hl=en" target="blank" class="me-4">Instagram</a>
<a href="https://www.youtube.com/channel/UC44Mzz2-5TpyfklUCQ5NuxQ" class="me-4">YouTube</a>
<a href="https://twitter.com/onebitcode">Twitter</a>
Style do projeto
Fazer o arquivo de variável de cor do projeto
Cor de hover de links: #b9b9b9
Cor de copyright da obc no footer: #555252
Cor do item da tabela: #d8d8d8
Padding fixo: 20px 0px
1. Criar uma pasta para as páginas
2. Fazer a criação do sass de cada página e fazer a criação do local onde terá os elementos comuns - Home, falcon9, humanSpace
3. Fazer a criação da pasta de comum elements
​4. Fazer a criação da estilização do header
​.header{
 font-size: 12px;
 font-weight: bold;
}
​5. Fazer agora a alteração de todos os container que temos, apra qe eles fique com as mesmas configurações, e depois a gente só precise fazer a adição dos backgrounds
​.container00 {
  min-height: 100vh;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
​6. Fazer agora a nossa alteração de arrow, para que ela fique centralizada, já que é um gif, não precisamos fazer nada alem de estilizar ela.
​.arrowDown {
  display: inline-block;
  width: 90px;
  margin-top: 5px;
}
7. Agora, nesse primeiro momento vamos fazer a alteração da logo no PC, depois disso vamos fazer a alteração da logo para resoluções menores.
.logoPc {
  width: 240px;
  margin-left: -10px;
  margin-right: 20px;
}
8. Agora iremos mexer na home de fato, vamos primeiramente colocar os backgrounds, como usaremos as heranças, faremos tudo dentro de container
.container00 {
  &.container01 {
    background-image: url(../imagens/home/01.jpg);
  }
  &.container02 {
    background-image: url(../imagens/home/03.jpg);
  }
  &.container03 {
    background-image: url(../imagens/home/02.gif);
  }
  &.container04 {
    background-image: url(../imagens/home/04.jpg);
  }
}
9. Faremos agora, alteração na nossa classe titlePadding, que é a classe que vamos ter em todos os títulos, com ela, iremos colocar um padding top para que ele fique com a distância que queremos
.titlePadding{
  padding-top: 200px;
}
10. Faremos alterações em shortTitle, e mediumTitle, que são os títulos que estão posicionados dentro da nossa página
.shortTitle {
  width: 550px;
  margin-bottom: -25px;
}
.mediumTitle {
  width: 650px;
  margin-bottom: -25px;
}
11. Agora iremos fazer mais algumas alterações no comumElements, para finalizamos, iremos alterar os botões
#button{
 padding: 15px 35px;
 border: 2px solid white;
}
12. E agora, iremos finalizar e ir para os media query dos elementos comuns e também específicos da nossa home.
.footer {
  background-color: black;
  height: 15vh;
  font-size: 12px;
  font-weight: 500;
  display: flex;
  align-items: center;
  justify-content: center;
  a {
    text-decoration: none;
    color: white;
    &:hover {
      color: $link-hover;
    }
  }
}
.copyOBC {
  color: $copy-obc;
}
13. Iremos fazer primeiramente dois, que será em 405px e em 350px, na parte de elementos comuns, alterando tamanhos no geral
@media (max-width: 405px) {
  .logoPc {
    width: 180px;
    margin-top: 15px;
  }
  .footer {
    font-size: 10px;
  }
}
@media (max-width: 350px) {
  .logoPc {
    width: 150px;
    margin-top: 15px;
 }
} ;
14. E agora faremos umas alterações em home, especificamente na parte de títulos, que fará com que a responsividade dos nossos títulos esteja completa.
@media (max-width: 750px) {
  .titlePadding {
    padding-top: 120px;
  }


  .shortTitle {
    width: auto;
    font-size: 50px;
  }


  .mediumTitle {
    width: auto;
    font-size: 50px;
  }
} ;
