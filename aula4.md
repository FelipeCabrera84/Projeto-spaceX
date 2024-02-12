1. Fazer a estilização de todos os containers, colocando background neles, também no carrossel
.container00 {
  &.container05 {
    background-image: url(../imagens/falcon9/01.jpg);
  }
  &.container06 {
    background-image: url(../imagens/falcon9/02.jpg);
  }
  &.carrossel01 {
    background-image: url(../imagens/falcon9/03.jpg);
  }
  &.carrossel02 {
    background-image: url(../imagens/falcon9/04.jpg);
  }
  &.carrossel03 {
    background-image: url(../imagens/falcon9/05.jpg);
  }
  &.carrossel04 {
    background-image: url(../imagens/falcon9/06.jpg);
  }
  &.carrossel05 {
    background-image: url(../imagens/falcon9/07.jpg);
  }
  &.container07 {
    background-image: url(../imagens/falcon9/08.jpg);
  }
}
2. Vamos fazer a alteração do titleContent, que é a classe primária do nosso container com textos
.titleContent {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 80vh;
}
3. Iremos fazer agora a alteração diretamente do title do nosso conteúdo.
.titleFalcon9 {
  font-size: 90px;
  font-family: "Rubik", sans-serif;
  font-weight: 514;
}
4. Agora faremos as alterações que precisamos nos números, fazendo com que eles fiquem do jeito que é necessário para termos os números certinhos​
.numbers {
  background-color: black;
  height: 40vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  h1 {
    font-size: 90px;
  }
  p {
    font-size: 20px;
  }
}
5. Iremos agora manipular o texto da descrição, para que ela tenha o que queremos
.falcon9Desc {
  font-size: 22px;
  width: 640px;
  line-height: 50px;
}
.containerFalcon9Desc {
  display: grid;
  height: 90vh;
  align-items: center;
  justify-content: left;
}
6. Manipularemos aqui agora algumas propriedades da tabela
#overViewPosition {
  width: 500px;
  margin-left: 13%;
  padding-top: 15%;
}
7. Faremos por último a manipulação dos slides, para que tenhamos os textos e o container de slide manipulado da melhor forma possível
.carrosselSlide {
  img {
    height: 100vh;
  }
}
8. Faremos agora a manipulação dos textos
.carousselText {
  background-color: black;
}
9. E agora, iremos finalizar e ir para os media query dos elementos comuns e também específicos da nossa home.
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
10. Vamos em commun elements para fazer a criação do nosso downloadDesc
.downloadDesc {
  background-color: black;
  height: 85vh;
  padding-top: 240px;
  a {
    text-decoration: none;
    color: $link-hover;
    &:hover {
      color: $table-item-color;
    }
  }
  button {
    border: 2px solid white;
    margin-right: 10px;
  }
}
11. Responsividade, começando pela página local, faremos 3 pontos de responsividade, 2 locais na falcon9 e 1 no communElements, esse será com 1024px de largura
@media (max-width: 1024px) {
  .numbers {
    p {
      font-size: 18px;
    }
  }
  .falcon9Desc {
    font-size: 26px;
  }
  #overViewPosition {
    display: block;
    width: 500px;
    margin-left: 13%;
    padding-top: 20%;
  }
}
12. Agora faremos com 425px de largura
@media (max-width: 425px) {
  .titleContent {
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-height: 80vh;
  }
  .titleFalcon9 {
    font-size: 50px;
  }
  .numbers {
    h1 {
      font-size: 40px;
    }
    p {
      font-size: 14px;
    }
  }
  .containerFalcon9Desc {
    p {
      width: auto;
      font-size: 18px;
      line-height: 30px;
    }
  }
  #overViewPosition {
    display: flex;
    height: 90vh;
    flex-direction: column;
    justify-content: center;
    width: auto;
    margin-left: auto;
  }
  .titleOverView {
    font-size: 26px;
    font-weight: bold;
  }
  .subTitleOvewView {
    font-size: 20px;
    font-weight: 300;
  }
}
13. Faremos uma de 510px de largura para o downloadDesc na área comum, pois iremos usar também no human
@media (max-width: 510px) {
  .downloadDesc {
    button {
      margin: 10px 0px;
    }
  }
}