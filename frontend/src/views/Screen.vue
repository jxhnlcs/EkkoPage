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
                <a href="">Peça Agora</a>
            </div>
        </div>
        <div id="um"></div>
    </div>
    <!--Por que escolher a ekko-->
    <div class="why">
        <div class="whyColumn">
            <h1>POR QUE ESCOLHER A EKKO ?</h1>
            <h2>Contamos com uma equipe de profissionais experientes e<br> apaixonados pela tecnologia, prontos para
                trabalhar
                em parceria<br> com você. Com uma abordagem colaborativa, entendemos suas<br> metas e desafios para criar
                sistemas inovadores que geram um<br> diferencial competitivo para o seu negócio.</h2>
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
        </div>
    </div>
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
    background-color: var(--tertiary-color);
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
    color: white;
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
    display: flex;
}

.why h1 {
    font-size: 38px;
    font-weight: 700;
    cursor: default;
    color: var(--primary-color);
}

.why h2 {
    font-size: 20px;
    cursor: default;
    font-weight: 400;
    line-height: normal;
    color: #526368;
    font-style: italic;
}

/* Soluções */

.solutionsSection {
    margin-top: 150px;
    text-align: center;
    background-color: var(--primary-color);
    position: relative;
}

.sistemas .solutionText {
    text-align: left;
    background-color: var(--tertiary-color);
    padding: 5px 30px;
    border-radius: 20px;
    box-shadow: 0 0.5rem 4rem rgba(197, 197, 197, 0.452);
    transition: 0.6s;
}

.sistemas .solutionText:hover {
    box-shadow: none;
}

.sites .solutionText:hover {
    box-shadow: none;
}

.sistemas,
.sites {
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

.solutions {
    display: flex;
    flex-direction: column;
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

.sites .solutionText {
    text-align: right;
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

.sistemas img,
.sites img {
    width: 850px;
    transition: transform 0.6s;
}

.sistemas img:hover,
.sites img:hover {
    transform: scale(1.1);
    /* Amplia a imagem em 10% */
}

.sistemas h2,
.sites h2 {
    color: var(--secondary-color);
    font-size: 2.0rem;
    cursor: default;
}

.sistemas h3,
.sites h3 {
    color: var(--secondary-color);
    font-size: 1.2rem;
    cursor: default;

}
</style>