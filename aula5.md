1. Vamos primeiro fazer o copy do HTML da página home, depois iremos começar o projeto.
2. Vamos agora fazer a parte 1 dos textos que temos
<div class="container text-center container01Content" data-aos="fade-down" data-aos-duration="1300">
                <h1>HUMAN SPACEFLIGHT</h1>
    
                <p>FAZENDO A VIDA MULTIPLANETÁRIA</p>
    
                <img src="/imagens/humanFlight/arrowDown.gif" alt="arrowDown" class="arrowDown" />
            </div>
3. Logo abaixo, vamos fazer uma descrição de terra, que será algo que é parecido com os numbers da página falcon9
<div class="container-fluid text-center eartDesc">
            <p data-aos="flip-right" data-aos-duration="1300">SpaceX também oferece voos cormeciais para orbita terrestre e
                lunar. Para começar a planejar a sua jornada,
                por favor contate-nos por <a href="#">onebitcode@gmail.com</a></p>
        </div>
4. Vamos agora fazer o segundo container da página, que será o container 09, o da terra
<div class="container-fluid container00 container09">
            <div class="containerRightContent" data-aos="fade-right" data-aos-duration="1500">
                <p>MISSAO</p>
                <h2 class="titleSection">ORBITA DA TERRA</h2>
                <p class="subTitle">EXPERIMENTE O PLANETA AZUL A 300KM DE ALTURA</p>
                <button type="button" class="btn btn-outline-light p-3 px-5">EXPLORAR</button>
            </div>
        </div>
5. Faremos agora o container10, que será o da estação espacial
<div class="container-fluid container00 container10">
            <div class="containerLeftContent" data-aos="fade-up" data-aos-duration="1600">
                <p>MISSAO</p>
                <h2 class="titleSection">ESTAÇÃO ESPACIAL</h2>
                <p class="subTitle">TRANSPORTANTO HUMANOS PARA O LABORATÓRIO VOADOR NO CÉU</p>
                <button type="button" class="btn btn-outline-light p-3 px-5">EXPLORAR</button>
            </div>
        </div>
6. Container11 da lua
<div class="container-fluid container00 container11">
            <div class="containerRightContent" data-aos="zoom-in-up" data-aos-duration="600">
                <p>MISSAO</p>
                <h2 class="titleSection">LUA</h2>
                <p class="subTitle">RETORNANDO HUMANOS PARA A NOSSA LUA VIZINHA</p>
                <button type="button" class="btn btn-outline-light p-3 px-5">EXPLORAR</button>
            </div>
        </div>
7. Container12, de marte
<div class="container-fluid container00 container12">
            <div class="containerLeftContent" data-aos="flip-right" data-aos-duration="1500">
                <p>MISSAO</p>
                <h2 class="titleSection">MARTE E ALÉM</h2>
                <p class="subTitle">O CAMINHO PARA TORNAR A HUMANIDADE MULTIPLANETÁRIA</p>
                <button type="button" class="btn btn-outline-light p-3 px-5">
                    EXPLORAR</button>
            </div>
        </div>
8. E agora iremos copiar o download desc que fizemos na página anterior para colocar aqui no final
<div class="container-fluid text-center downloadDesc">
            <p data-aos="fade-right" data-aos-duration="1200"><span>Para mais informações sobre os serviçoes entre em
                    contato
                    com</span> <a href="https://www.instagram.com/onebitcode/" target="blank">onebitcode@gmail.com</a></p>
    
            <button type="button" class="btn btn-outline-light p-3" data-aos="flip-left" data-aos-duration="1000">BAIXAR
                GUIA DO USUÁRIO</button>
            <button type="button" class="btn btn-outline-light p-3" data-aos="flip-up" data-aos-duration="1300">CAPACIDADES
                E
                SERVIÇOS</button>
        </div>
Style do projeto
1. Faremos as esilizações de todos os containers
.container00 {
      &.container08 {
        background-image: url(../imagens/humanFlight/01.jpg);
      }
    
      &.container09 {
        background-image: url(../imagens/humanFlight/02.jpg);
      }
    
      &.container10 {
        background-image: url(../imagens/humanFlight/03.jpg);
      }
    
      &.container11 {
        background-image: url(../imagens/humanFlight/04.jpg);
      }
    
      &.container12 {
        background-image: url(../imagens/humanFlight/05.jpg);
      }
    }
2. Agora faremos do container01Content, que com ele nós faremos a estilização do texto do container01 da página human
    .container01Content {
      height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    
      h1 {
        font-size: 120px;
      }
    
      p {
        margin-top: 20px;
        margin-bottom: 50px;
        font-size: 30px;
        font-weight: 300;
      }
    
      img {
        width: 130px;
      }
    }
    
3. Agora faremos da descrição da terra
    .eartDesc {
      background-color: black;
      height: 25vh;
      display: flex;
      align-items: center;
      justify-content: center;
    
      p {
        color: $table-item-color;
        font-weight: 400;
        font-size: 20px;
        width: 800px;
      }
    
      a {
        text-decoration: none;
        color: white;
        font-weight: 500;
      }
    }
    
4. Agora faremos a estilização de todos os conteúdos que vão ficar na direita da página
    .containerRightContent {
      margin-left: 55%;
      padding-top: 15%;
    }
    
5. Mexeremos agora na classe title e também de subtitle
    .titleSection {
      font-size: 60px;
      font-weight: bold;
    }
    
    .subTitle {
      font-weight: 300;
      margin-bottom: 40px;
    }
    
6. Por último faremos a manipulação dos conteúdos da parte left
    .containerLeftContent {
      margin-left: 5%;
      padding-top: 15%;
    }
    
7. Faremos agora a manipulação de conteúdos nos mediaQuery 1024
    @media (max-width: 1024px) {
      .container01Content {
        h1 {
          font-size: 90px;
        }
    
        p {
          margin: 20px 0px;
          font-size: 30px;
          font-weight: 300;
        }
      }
    
      .containerRightContent {
        margin-left: 50%;
        padding-top: 20%;
      }
    
      .titleSection {
        font-size: 50px;
        font-weight: bold;
      }
    
      .subTitle {
        font-weight: 300;
        margin-bottom: 40px;
      }
    
      .containerLeftContent {
        margin-left: 5%;
        padding-top: 20%;
      }
    }
    
8. Faremos agora a manipulação de conteúdos nos mediaQuery 425
    @media (max-width: 425px) {
      .container01Content {
        h1 {
          font-size: 40px;
        }
    
        p {
          font-size: 16px;
        }
      }
    
      .arrowDown {
        display: none;
      }
    
      .eartDesc {
        height: 30vh;
        p {
          color: $table-item-color;
          font-weight: 400;
          font-size: 14px;
          width: auto;
        }
      }
    
      .containerRightContent {
        margin-left: 20%;
        padding-top: 30%;
      }
    
      .titleSection {
        font-size: 50px;
        font-weight: bold;
      }
    
      .subTitle {
        font-weight: 300;
        margin-bottom: 40px;
      }
    
      .containerLeftContent {
        margin-left: 7%;
        padding-top: 30%;
      }
    }
    
