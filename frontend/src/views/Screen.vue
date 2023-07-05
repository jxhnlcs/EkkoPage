<template>
    <!--Nav-->
    <div class="header">
        <nav>
            <div class="logo">
                <img src="../assets/img/ekkosemfundo.png" alt="logo"> <!--ADICIONAR LOGO-->
            </div>
            <ul id="navbar">
                <li><a href="#um">Sobre</a></li>
                <li><a href="#dois">Soluções</a></li>
                <li><a href="#tres">Contato</a></li>
            </ul>
        </nav>
        <!--Main-->
        <div class="main">
            <img src="../assets/img/ekkosemfundo.png" alt="">
            <div>
                <h1><span>AUTOMATIZE</span><br>processos e ganhe tempo com<br>nossas soluções inteligentes<br></h1>
                <a href="https://api.whatsapp.com/send/?phone=557592868576&text&type=phone_number&app_absent=0">Peça Agora</a>
            </div>
        </div>
        <div></div>
    </div>
    <div id="um"></div>
    <!--Por que escolher a ekko-->
    <div class="why">
        <div class="whyRow">
            <div class="whyColumn">
                <h1>VANTAGENS DA EKKO </h1>
                <h2>Contamos com uma equipe de profissionais experientes e<br> apaixonados pela tecnologia, prontos para
                    trabalhar
                    em parceria<br> com você. Com uma abordagem colaborativa, entendemos suas<br> metas e desafios para
                    criar
                    sistemas inovadores que geram um<br> diferencial competitivo para o seu negócio.</h2>
            </div>
            <img src="../assets/img/team-animate.svg">
        </div>
        <div class="icons">
            <div class="icon">
                <a href="">
                    <span class="material-symbols-sharp">
                        verified
                    </span>
                </a>
                <h3>Experiência<br>Especializada</h3>
            </div>
            <div class="icon">
                <a href=""><span class="material-symbols-sharp">
                        target
                    </span></a>
                <h3>Abordagem centrada<br> ao cliente</h3>
            </div>
            <div class="icon">
                <a href=""><span class="material-symbols-sharp">
                        brush
                    </span></a>
                <h3>Design atraente<br> e intuitivo</h3>
            </div>
            <div class="icon">
                <a href=""><span class="material-symbols-sharp">
                        construction
                    </span></a>
                <h3>Suporte e<br> Manutenção</h3>
            </div>
        </div>
    </div>

    <!--Soluções-->
    <div id="dois" class="solutionsSection">
        <h1>Nossas Soluções</h1>
        <div class="solutions">
            <div class="sistemas">
                <img src="../assets/img/sistema.png" alt="">
                <div class="solutionText">
                    <h2>Sistemas de Gerenciamento</h2>
                    <h3>Desenvolvemos sistemas de gestão sob medida<br> para impulsionar o sucesso de qualquer<br> segmento
                        de
                        empresa</h3>
                </div>
            </div>
            <div class="sites">
                <div class="solutionText">
                    <h2>Landing Page</h2>
                    <h3>Transforme sua presença online com landing pages<br> impactantes e envolventes, criadas por nossa
                        equipe<br>
                        especializada em design e desenvolvimento</h3>
                </div>
                <img src="../assets/img/landingPage.png" alt="">
            </div>
            <div class="aplicativos">
                <img src="../assets/img/aplicativo.png" alt="">
                <div class="solutionText">
                    <h2>Aplicativos</h2>
                    <h3>Explore novas possibilidades com<br>aplicativos inovadores, desenvolvidos<br> para facilitar a
                        experiência do usuário e<br>impulsionar o crescimento do seu negócio</h3>
                </div>
            </div>
        </div>
    </div>

    <!--Contate-nos-->

    <div id="tres" class="contatoSection">
        <div class="contatoRow">
            <div class="contatoColumn">
                <h1>Contate-nos</h1>
                <h2>Tire dúvidas ou planeje um orçamento.<br>Nossa equipe especializada está pronta<br>para esclarecer todas
                    as suas dúvidas e<br>fornecer informações detalhadas sobre<br>nossos produtos e serviços.</h2>
                <div class="contatoIcons">
                    <a href="https://api.whatsapp.com/send/?phone=557592868576&text&type=phone_number&app_absent=0"><img src="../assets/img/whatsapp.png" alt="Whatsapp icon"></a>
                    <a href="https://www.instagram.com/ekko.sistemas/"><img src="../assets/img/instagram.png" alt="Instagram icon"></a>
                    <a href="mailto:ekkosistemas@outlook.com"><img src="../assets/img/outlook.png" alt="Outlook icon"></a>
                </div>
            </div>
            <img src="../assets/img/contact-us-animate.svg" alt="">
        </div>
    </div>

    <!--Footer-->
    <footer>
        <div class="bottom-details">
            <div class="bottom_text">
                <span class="copyright_text">Copyright © 2023 Ekko. Todos os direitos reservados</span>
            </div>
        </div>
    </footer>
</template>

<style>
.header {
    height: 750px;
    width: 100%;
    background: url(../assets/img/casalLaptop.png);

    position: relative;
}

.logo {
    display: flex;
    justify-content: center;
    align-items: center;
}

.header nav {
    width: 90%;
    margin: auto;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0.5rem 0 2rem;
}

.header .menu {
    font-size: 25px;
    display: none;
}

.header nav img {
    width: 120px;
    margin-right: 650px;
}

.header nav ul {
    display: flex;
}

.header nav li {
    list-style: none;
    margin: 0 5px;
}

.header nav li a {
    text-decoration: none;
    text-transform: uppercase;
    padding: 0.2rem 1rem;
    font-size: 15px;
    font-weight: bold;
    color: var(--secondary-color);
    position: relative;
    z-index: 1;
}

.header nav li a::before {
    content: '';
    width: 0%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background-color: var(--primary-color);
    border-radius: 20px;
    z-index: -1;
    transition: 0.5s linear;
}

.header nav li a:hover:before {
    width: 100%;
}

.header .main {
    display: flex;
    justify-content: space-around;
}


.main h1 {
    color: var(--secondary-color);
    cursor: default;
}

.main a {
    margin-top: 30px;
    text-decoration: none;
    color: var(--primary-color);
    background-color: var(--secondary-color);
    padding: 15px;
    border-radius: 20px;
    margin-left: 600px;
    font-weight: bold;
    transition: background-color 0.3s ease-in-out, color 0.3s ease-in-out;
}

.main a:hover {
    color: var(--tertiary-color);
}


.main a:hover {
    background-color: var(--secondary-color);
}

.header .main span {
    font-size: 100px;
}

.header .main h1 {
    font-size: 2.5rem;
    margin-top: 70px;
    font-family: 'Montserrat', sans-serif;
    margin-bottom: 2rem;
    text-align: right;
}

.header .main img {
    width: 400px;
    border-radius: 300px;
}

/* Por que escolher */

.why {
    margin-top: 60px;
}

.whyRow {
    display: flex;
    justify-content: center;
    align-items: center;

}

.why h1 {
    font-size: 48px;
    font-weight: 700;
    cursor: default;
    color: var(--primary-color);
}

.whyRow img {
    margin-left: 50px;
    width: 700px;
}

.why h2 {
    font-size: 28px;
    cursor: default;
    font-weight: 400;
    line-height: normal;
    color: var(--quarter-color);
    font-style: italic;
}

.icons {
    margin-top: 20px;
    display: flex;
    justify-content: space-around;
}

.icons .icon {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.icons a {
    background-color: var(--primary-color);
    padding: 50px 55px;
    border-radius: 50px;
    transition: background-color 0.3s ease-in-out, color 0.3s ease-in-out;
}

.icon h3 {
    font-size: 22px;
    color: var(--primary-color);
    text-align: center;
    text-transform: uppercase;
}

.icons a span {
    font-size: 60px;
    color: var(--secondary-color)
}

.icons a:hover {
    background-color: var(--tertiary-color);

}

/* Soluções */

.solutionsSection {
    margin-top: 150px;
    text-align: center;
    background: rgb(0, 136, 181);
    background: linear-gradient(180deg, rgba(0, 136, 181, 1) 50%, rgba(0, 54, 108, 1) 84%);
    position: relative;
}

.solutionsSection h1 {
    color: var(--secondary-color);
    font-size: 2.8rem;
    padding: 25px;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    cursor: default;
}

.solutions {
    display: flex;
    flex-direction: column;
}

.sistemas,
.sites,
.aplicativos {
    margin-top: 150px;
    display: inline-block;
    text-align: center;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

.sites {
    margin-top: -30px;
}

.aplicativos {
    margin-top: -30px;
}

.sistemas .solutionText {
    text-align: left;
    background-color: var(--tertiary-color);
    padding: 5px 30px;
    border-radius: 20px;
    box-shadow: 0 0.5rem 4rem rgba(197, 197, 197, 0.452);
    transition: 0.6s;
}

.sistemas .solutionText h2 {
    font-size: 30px;
}

.sistemas .solutionText h3 {
    font-size: 28px;
    font-style: italic;
    font-weight: 100;
}


.sites .solutionText {
    text-align: left;
    background-color: var(--tertiary-color);
    padding: 5px 30px;
    border-radius: 30px;
    box-shadow: 0 0.5rem 4rem rgba(197, 197, 197, 0.452);
    transition: 0.6s;
}

.sites .solutionText h2 {
    font-size: 30px;
}

.sites .solutionText h3 {
    font-size: 28px;
    font-style: italic;
    font-weight: 100;
}

.aplicativos .solutionText {
    text-align: left;
    background-color: var(--tertiary-color);
    padding: 5px 30px;
    border-radius: 20px;
    box-shadow: 0 0.5rem 4rem rgba(197, 197, 197, 0.452);
    transition: 0.6s;
}

.aplicativos .solutionText h2 {
    font-size: 30px;
}

.aplicativos .solutionText h3 {
    font-size: 28px;
    font-style: italic;
    font-weight: 100;
}

.sites .solutionText {
    text-align: right;
}

.sistemas .solutionText:hover {
    box-shadow: none;
}

.sites .solutionText:hover {
    box-shadow: none;
}

.aplicativos .solutionText:hover {
    box-shadow: none;
}

.sistemas img,
.sites img,
.aplicativos img {
    width: 850px;
    transition: transform 0.6s;
}

.sistemas img:hover,
.sites img:hover,
.aplicativos img:hover {
    transform: scale(1.1);
    /* Amplia a imagem em 10% */
}

.sistemas h2,
.sites h2,
.aplicativos h2 {
    color: var(--secondary-color);
    font-size: 2.0rem;
    cursor: default;
}

.sistemas h3,
.sites h3,
.aplicativos h3 {
    color: var(--secondary-color);
    font-size: 1.2rem;
    cursor: default;
}

.contatoSection{
    margin-top: 60px;
}

.contatoRow{
    display: flex;
    /* justify-content: center; */
    justify-content: space-around;
    
}

.contatoRow h1 {
    font-size: 48px;
    font-weight: 700;
    cursor: default;
    color: var(--primary-color);
}

.contatoRow img {
    /* margin-left: 50px; */
    width: 500px;
}

.contatoRow h2 {
    font-size: 28px;
    cursor: default;
    font-weight: 400;
    line-height: normal;
    color: var(--primary-color);
    font-style: italic;
}

.contatoIcons{
    display: flex;
    justify-content: start;
    margin-top: 15px;
}


.contatoIcons a img{
    width: 65px;
    margin-right: 39px;
    border-radius: 50%;
}

/* Footer */

footer .bottom-details{
  width: 100%;
  background: var(--primary-color);
  display: flex;
  align-items: center;
}
footer .bottom-details .bottom_text{
  margin: auto;
  padding: 20px 40px;
  display: flex;
  justify-content: space-between;
}
.bottom-details .bottom_text span,
.bottom-details .bottom_text a{
  font-size: 14px;
  color: var(--secondary-color);
  font-weight: bold;
  text-decoration: none;
}
.bottom-details .bottom_text a:hover{
  opacity: 1;
  text-decoration: underline;
}
.bottom-details .bottom_text a{
  margin-right: 10px;
}


</style>