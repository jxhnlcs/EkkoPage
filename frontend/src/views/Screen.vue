<template>
    <!--Nav-->
    <div class="header">
        <nav>
            <div class="logo">
                <img src="../assets/img/ekko.png" alt="logo"> <!--ADICIONAR LOGO-->
            </div>
            <ul id="navbar">
                <li><a href="#um">Sobre</a></li>
                <li><a href="#dois">Soluções</a></li>
                <li><a href="#tres">Contato</a></li>
            </ul>
        </nav>
        <!--Main-->
        <div class="main">
            <img src="../assets/img/ekkoWhite.png" alt="">
            <div>
                <h1><span>AUTOMATIZE</span><br>processos e ganhe tempo com<br>nossas soluções inteligentes<br></h1>
                <a href="">Peça Agora</a>
            </div>
        </div>
    </div>
    <!--Por que escolher a ekko-->
    <div class="why">
        <h1>POR QUE ESCOLHER A EKKO ?</h1>
        <h2>Contamos com uma equipe de profissionais experientes e<br> apaixonados pela tecnologia, prontos para trabalhar em parceria<br> com você. Com uma abordagem colaborativa, entendemos suas<br> metas e desafios para criar sistemas inovadores que geram um<br> diferencial competitivo para o seu negócio.</h2>
    </div>

    <!--Soluções-->
    <div class="solutions">
        <h1>Nossas Soluções</h1>
        <div class="sistemas">
            <h2>Sistemas</h2>
            <img src="../assets/img/dispositivos.png" alt="">
            <h3>Desenvolvemos sistemas de gestão sob medida<br> para impulsionar o sucesso de qualquer<br> segmento de empresa</h3>
        </div>
        <div class="sites">
            <h2>Sites</h2> 
            <img src="../assets/img/dispositivos.png" alt="">
            <h3>Transforme sua presença online com landing pages<br> impactantes e envolventes, criadas por nossa equipe<br> especializada em design e desenvolvimento</h3>
        </div>
        
    </div>

</template>

<style>
.header {
    height: 80vh;
    width: 100%;
    background-color: var(--primary-color);
    position: relative;
}

.logo{
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
    color: var(--tertiary-color);
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
    background-color: var(--secondary-color);
    border-radius: 20px;
    z-index: -1;
    transition: 0.5s linear;
}

.header nav li a:hover:before {
    width: 100%;
}

.header nav li a:hover {
    color: var(--primary-color);
}

.header .main {
    display: flex;
    justify-content: space-around;
}


.main h1 {
    color: white;
}

.main a{
    margin-top: 30px;
    text-decoration: none;
    color: var(--primary-color);
    background-color: var(--secondary-color);
    padding: 15px;
    border-radius: 20px;
    margin-left: 600px;
    transition: background-color 0.3s ease-in-out, color 0.3s ease-in-out;
    
}


.main a:hover{
    background-color: white;
}

.header .main span{
    font-size: 100px;
}

.header .main h1 {
    font-size: 2.5rem;
    margin-top: 70px;
    font-family: 'Montserrat', sans-serif;
    margin-bottom: 2rem;
    text-align: right;
}

.header .right-box {
    position: absolute;
    right: 0;
    bottom: 0;
}

.header .right-box img {
    width: 100%;
}

/* Por que escolher */
.why{
    margin-top: 130px;
    color: var(--primary-color);
    text-align: center;
}

.why h1{
    font-size: 60px;
}

.why h2{
    font-size: 30px;
}


.solutions {
  margin-top: 150px;
  text-align: center;
  background-color: var(--primary-color);
  height: 90vh;
  position: relative;
}

.solutions h1 {
  color: white;
  font-size: 2.8rem;
  padding: 25px;
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
}

.sistemas,
.sites {
  margin-top: 150px;
  display: inline-block;
  text-align: center;
}

.sistemas {
  margin-right: 200px;
}

.sistemas img,
.sites img {
  width: 700px;
  transition: transform 0.6s; /* Adiciona uma transição suave para o efeito */
}

.sistemas img:hover,
.sites img:hover {
  transform: scale(1.1); /* Amplia a imagem em 10% */
}

.sistemas h2,
.sites h2 {
  color: white;
  font-size: 2.0rem;
}

.sistemas h3,
.sites h3 {
  color: white;
  font-size: 1.2rem;
}

</style>