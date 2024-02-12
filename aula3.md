HTML do Projeto

1. Vamos primeiramente copiar todo o HTML da página home, para deixarmos já algumas coisas como padrão, como o footer e o header, assim também como alguns containers.
2. Vamos fazer a mudança de container01 para container05 e com isso vamos colocar dentro desse container mais um, onde ficaram os elementos.
<div class="container text-center titleContent" data-aos="fade-up" data-aos-duration="1500">
         <h1 class="titleFalcon9">FALCON 9</h1>
         <p class="h5 subTitleFalcon">PRIMEIRA CLASSE DE FOGUETES DE ORBITA CAPAZ DE VOLTAR</p>
    </div>
3. Faremos mais abaixo, um container fluid para os números, aqui usaremos o grid do Bootstrap
<div class="container-fluid numbers">
</div>
4. Iremos criar uma div com linha e 3 colunas, que elas vão ter as suas classes.
<div class="row text-center">
        <div class="col-sm col1">
            <h1 class="titleNumb" data-aos="flip-up" data-aos-duration="1000">126</h1>
            <p class="subTitleNumb" data-aos="flip-up" data-aos-duration="1000">LANÇAMENTOS TOTAIS</p>
        </div>
        <div class="col-sm">
            <h1 class="titleNumb" data-aos="flip-left" data-aos-duration="1000">86</h1>
            <p class="subTitleNumb" data-aos="flip-left" data-aos-duration="1000">DESEMBARQUES TOTAIS</p>
        </div>
        <div class="col-sm col3">
            <h1 class="titleNumb" data-aos="flip-right" data-aos-duration="1000">68</h1>
            <p class="subTitleNumb" data-aos="flip-right" data-aos-duration="1000">FOGUETES RECUPERADOS</p>
        </div>
    </div>
5. Agora iremos criar um container06, que terá nele os elementos abaixo dos números na página principal
<div class="container-fluid container00 container06">
    <div class="container containerFalcon9Desc">
        <p class="falcon9Desc" data-aos="fade-right" data-aos-duration="1500">
            O Falcon 9 é um foguete reutilizável de dois estágios projetado e fabricado pela SpaceX para o
            transporte confiável e seguro de pessoas e cargas úteis para a órbita da Terra e além. Falcon 9 é o
            primeiro foguete reutilizável de classe orbital do mundo. A capacidade de reutilização permite que a
            SpaceX refile as partes mais caras do foguete, o que, por sua vez, reduz o custo do acesso ao espaço.
        </p>
    </div>
</div>
6. Agora iremos para a parte do carrossel, iremos pegar um carrossel qualquer no Bootstrap, que nesse caso usamos um padrão com indicadores para passarmos e ao invés de colocarmos imagens dentro dos carrossel item, iremos colocar textos, e usaremos o background para as imagens
<div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active container00 carrossel01" data-bs-interval="3000000">
                <div class="container" id="overViewPosition">
                    <p class="subTitleOvewView">FALCON 9</p>
                    <h3 class="titleOverView">VISÃO GERAL</h3>
                    <table class="table" id="widthTable">
                       <tbody>
                            <tr data-aos="fade-right" data-aos-duration="1500">
                                <td>ALTURA</td>
                                <td class="text-end">70 m<span class="corEscuraTxt">/ 229.6 f</span></td>
                            </tr>
                             <tr data-aos="fade-right" data-aos-duration="1200">
                                <td>DIAMETRO</td>
                                <td class="text-end">3.7 m<span class="corEscuraTxt"> / 12 ft</span></td>
                             </tr>
                            <tr data-aos="fade-right" data-aos-duration="1500">
                                <td>MASSA</td>
                                <td class="text-end">549,054 kg<span class="corEscuraTxt"> / 1,207,920 lb</span></td>
                            </tr>
                            <tr data-aos="fade-right" data-aos-duration="1400">
                                <td>CARGA MÁXIMA PARA LEO</td>
                                <td class="text-end">22,800 kg<span class="corEscuraTxt"> / 50,265 lb</span></td>
                            </tr>
                            <tr data-aos="fade-right" data-aos-duration="1600">
                                <td>CARGA MÁXIMA PARA GTO</td>
                                <td class="text-end">8,300 kg<span class="corEscuraTxt"> / 18,300 lb</span></td>
                            </tr>
                            <tr data-aos="fade-right" data-aos-duration="1300">
                                <td>CARGA MÁXIMA PARA MARTE</td>
                                <td class="text-end">4,020 kg<span class="corEscuraTxt"> / 8,860 lb</span></td>
                            </tr>
                     </tbody>
                     </table>
                </div>
            </div>
            <div class="carousel-item container00 carrossel02" data-bs-interval="3000000">
               <div class="container" id="overViewPosition">
                    <p class="subTitleOvewView">FALCON 9</p>
                    <h3 class="titleOverView">PRIMEIRO ESTÁGIO</h3>
                     <p>
                        Falcon 9's O primeiro estágio do Falcon 9 incorpora nove motores Merlin e tanques de liga de
                        alumínio-lítio
                        contendo oxigênio líquido e propelente de querosene de grau de foguete (RP-1).
                     </p>
                    <p>
                        O Falcon 9 gera mais de 1,7 milhão de libras de empuxo ao nível do mar.
                    </p>
                 </div>
            </div>
            <div class="carousel-item container00 carrossel03" data-bs-interval="3000000">
                 <div class="container" id="overViewPosition">
                    <p class="subTitleOvewView">FALCON 9</p>
                    <h3 class="titleOverView">SEGUNDO ESTÁGIO</h3>
                    <p>
                        O segundo estágio, alimentado por um único motor a vácuo Merlin, entrega a carga útil do Falcon
                        9 à órbita desejada. O motor do segundo estágio acende alguns segundos após a separação do
                        estágio e pode ser reiniciado várias vezes para colocar várias cargas em diferentes órbitas.
                    </p>
                    <table class="table" id="widthTable">
                      <tbody>
                             <tr>
                                <td>NÚMERO DE MOTORES</td>
                                <td class=" text-end">1 vacuum</td>
                             </tr>
                             <tr>
                                <td>TEMPO DE QUEIMA</td>
                                <td class=" text-end">397seg</td>
                             </tr>
                             <tr>
                                <td>IMPULSO</td>
                                <td class=" text-end">981 kN <span>/ 220.500 lbf</span></td>
                             </tr>
                       </tbody>
                   </table>
               </div>
           </div>
             <div class="carousel-item container00 carrossel04" data-bs-interval="2000000">
                <div class="container" id="overViewPosition">
                    <p class="subTitleOvewView">FALCON 9</p>
                    <h3 class="titleOverView">INTERESTADUAL</h3>
                    <p>
                        A interestadual é uma estrutura composta que conecta o primeiro e o segundo estágios e abriga os
                        empurradores pneumáticos que permitem que o primeiro e o segundo estágios se separem durante o
                        vôo.
                    </p>
                    <p style="font-size: 18px;">ALETAS DE GRADE</p>
                    <p>
                        O Falcon 9 está equipado com quatro aletas de grade hipersônicas posicionadas na base da
                        interestadual. Eles orientam o foguete durante a reentrada, movendo o centro de pressão.
                    </p>
               </div>
            </div>
            <div class="carousel-item container00 carrossel05" data-bs-interval="3000000">
               <div class="container" id="overViewPosition">
                    <p class="subTitleOvewView">FALCON 9</p>
                    <h3 class="titleOverView">CARGA ÚTIL</h3>
                    <p>
                        Feita de um material composto de carbono, a carenagem protege os satélites em seu caminho para a
                        órbita. A carenagem é lançada a aproximadamente 3 minutos em vôo, e a SpaceX continua a
                        recuperar as carenagens para reutilização em missões futuras.
                    </p>
                    <table class="table" id="widthTable">
                        <tbody>
                            <tr>
                                <td>ALTURA</td>
                                <td class=" text-end">13,1m <span>/43 ft</span></td>
                            </tr>
                            <tr>
                                <td>DIÂMETRO</td>
                                <td class=" text-end">5,2m <span>/17,1 ft</span></td>
                            </tr>
                        </tbody>
                   </table>
               </div>
          </div>
         </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
7. Esse foi o primeiro item do carrossel, que foi uma tabela, usada para colocar os itens que temos aqui, iremos para o segundo item do carrossel
<div class="carousel-item container00 carrossel02" data-bs-interval="3000000">
            <div class="container" id="overViewPosition">
                <p class="subTitleOvewView">FALCON 9</p>
                <h3 class="titleOverView">PRIMEIRO ESTÁGIO</h3>
                 <p>
                    Falcon 9's O primeiro estágio do Falcon 9 incorpora nove motores Merlin e tanques de liga de
                    alumínio-lítio
                    contendo oxigênio líquido e propelente de querosene de grau de foguete (RP-1).
                 </p>
                <p>
                    O Falcon 9 gera mais de 1,7 milhão de libras de empuxo ao nível do mar.
                </p>
           </div>
        </div>
8. Terceiro item do carrossel
<div class="carousel-item container00 carrossel03" data-bs-interval="3000000">
            <div class="container" id="overViewPosition">
                <p class="subTitleOvewView">FALCON 9</p>
                <h3 class="titleOverView">SEGUNDO ESTÁGIO</h3>
                <p>
                    O segundo estágio, alimentado por um único motor a vácuo Merlin, entrega a carga útil do Falcon
                    9 à órbita desejada. O motor do segundo estágio acende alguns segundos após a separação do
                    estágio e pode ser reiniciado várias vezes para colocar várias cargas em diferentes órbitas.
                </p>
                <table class="table" id="widthTable">
                    <tbody>
                        <tr>
                            <td>NÚMERO DE MOTORES</td>
                            <td class=" text-end">1 vacuum</td>
                        </tr>
                        <tr>
                            <td>TEMPO DE QUEIMA</td>
                            <td class=" text-end">397seg</td>
                        </tr>
                        <tr>
                            <td>IMPULSO</td>
                            <td class=" text-end">981 kN <span>/ 220.500 lbf</span></td>
                        </tr>
                   </tbody>
               </table>
           </div>
       </div>
9. Quarto item do carrossel
<div class="carousel-item container00 carrossel04" data-bs-interval="2000000">
            <div class="container" id="overViewPosition">
                <p class="subTitleOvewView">FALCON 9</p>
                <h3 class="titleOverView">INTERESTADUAL</h3>
                 <p>
                    A interestadual é uma estrutura composta que conecta o primeiro e o segundo estágios e abriga os
                    empurradores pneumáticos que permitem que o primeiro e o segundo estágios se separem durante o
                    vôo.
                 </p>
                <p style="font-size: 18px;">ALETAS DE GRADE</p>
                <p>
                    O Falcon 9 está equipado com quatro aletas de grade hipersônicas posicionadas na base da
                    interestadual. Eles orientam o foguete durante a reentrada, movendo o centro de pressão.
                </p>
           </div>
        </div>
10. Quinto item do carrossel
<div class="carousel-item container00 carrossel05" data-bs-interval="3000000">
           <div class="container" id="overViewPosition">
                <p class="subTitleOvewView">FALCON 9</p>
                <h3 class="titleOverView">CARGA ÚTIL</h3>
                <p>
                    Feita de um material composto de carbono, a carenagem protege os satélites em seu caminho para a
                    órbita. A carenagem é lançada a aproximadamente 3 minutos em vôo, e a SpaceX continua a
                    recuperar as carenagens para reutilização em missões futuras.
                </p>
                <table class="table" id="widthTable">
                     <tbody>
                        <tr>
                            <td>ALTURA</td>
                            <td class=" text-end">13,1m <span>/43 ft</span></td>
                        </tr>
                        <tr>
                            <td>DIÂMETRO</td>
                            <td class=" text-end">5,2m <span>/17,1 ft</span></td>
                        </tr>
                    </tbody>
               </table>
           </div>
        </div>
11. Agora temos o container 07, que tem outro texto
<div class="container-fluid container00 container07">
         <div class="container" id="overViewPosition" data-aos="fade-right" data-aos-duration="1400">
            <p class="subTitleOvewView">FALCON 9</p>
            <h3 class="titleOverView">MERLIN</h3>
            <p>
                Merlin é uma família de motores de foguete desenvolvidos pela SpaceX para uso em seus veículos de
                lançamento Falcon 1, Falcon 9 e Falcon Heavy. Os motores Merlin usam querosene de grau de foguete (RP-1)
                e oxigênio líquido como propelentes de foguete em um ciclo de energia de gerador a gás. O motor Merlin
                foi originalmente projetado para recuperação e reutilização.
            </p>
            <table class="table" id="widthTable">
                <tbody>
                    <tr>
                        <td>PROPULSOR</td>
                        <td class="text-end">LOX <span>/ RP-1</span></td>
                    </tr>
                    <tr>
                        <td>IMPULSO</td>
                        <td class=" text-end">845 kN <span>/ 190.000 lbf</span></td>
                    </tr>
               </tbody>
           </table>
       </div>
    </div>
12. Faremos agora o uso de outro carrossel, esse carrossel terá textos, marcadores abaixo do texto e dos lados também, com isso, vamos colocar a imagem diretamente no carrossel, não no background
<div id="carouselExampleCaptions" class="carousel slide carrosselSlide" data-bs-ride="carousel">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                aria-label="Slide 3"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="3"
                aria-label="Slide 4"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="4"
                aria-label="Slide 5"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="5"
                aria-label="Slide 6"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active" data-bs-interval="1000000">
                <img src="/imagens/falcon9/09.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                    <p class="carousselText">O Falcon 9 lança o Dragon para a Estação Espacial Internacional do Complexo
                        de
                        Lançamento 39A</p>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="2000000">
                <img src="/imagens/falcon9/10.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                   <p class="carousselText">Primeiro e segundo estágio após a separação de voo</p>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="3000000">
                <img src="/imagens/falcon9/11.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                    <p class="carousselText">Falcon 9 decola com sua carga útil Iridium-5</p>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="3000000">
                <img src="/imagens/falcon9/12.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                    <p class="carousselText">Falcon 9 pousando no droneship para ler as instruções</p>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="3000000">
                <img src="/imagens/falcon9/13.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                      <p class="carousselText">Clone dos motores Merlin do Falcon 9 durante a decolagem</p>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="3000000">
                <img src="/imagens/falcon9/14.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-md-block">
                    <p class="carousselText">O falcon 9 deixa um rastro de luz ao decolar da Base Aérea de Vandenberg
                    </p>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
13. Teremos aqui, antes do footer, um espaço para ter esse download desc, que terá o “complemento” do que temos aqui no footer
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