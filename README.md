PAGINA 1

<!DOCTYPE html>
<html lang="pt-br">  <!--LINGUAGEM DA PAGINA-->
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio</title>
    <link rel="stylesheet" href="./styles/style.css">  <!-- SERVE PARA LINKAR A PAGINA HML COM A CSS-->
</head>
<body>
      <header class="cabecalho">
        <nav class="cabecalho_menu">
            <a class="cabecalho_menu_link" href="index.html"> Home</a>
            <a class="cabecalho_menu_link" href="about.html">Sobre mim</a>
        </nav>
      </header>
      <main class="apresentacao">
            <section class="apresentacao__conteudo">
                <h1 class="apresentacao__titulo">Eleve seu negócio digital a outro nível <strong class="titulo-destaque"> com um Front-end de qualidade!</strong> </h1> <!--ADCIONAR O CLASS NO STRONG PARA ESPECIFICAR O LOCAL QUE SERA EDITADO-->

                <p class="apresentacao__conteudo__texto">Olá! Sou o Ryan Pelais, desenvolvedor Front-end com especialidade em React, HTML e CSS. Ajudo pequenos negócios e designers a colocarem em prática boas ideias. Vamos conversar?</p>
                <div class="apresentacao__links">
                    <h2 class="apresentacao_links_subtitulo">Acesse minhas redes:</h2>
                    
                    <a class="apresentacao__links__links" href="https://Instagram.com/ryanpelais"> <img src="./assets/instagram.png"> Instagram</a>

                    <a class="apresentacao__links__links" href="https://github.com/ryanpelais"> <img src="./assets/github.png"> Github </a>

                    <a class="apresentacao__links__links" href="https://www.linkedin.com/in/ryan-pelais-b5b4ab233/"> <img src="./assets/linkedin.png">Linkedin</a>
                </div>
            </section>
            <img src="./assets/img2.png" alt="Foto de Perfil do Ryan">

      </main>
      <footer class="rodape">
        <p>Desenvolvido por Ryan Pelais.</p>
      </footer>
</body>
</html>


PAGINA 2

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sobre mim</title>
   <link rel="stylesheet" href="./styles/style.css" >
</head>
<body>
    <header class="cabecalho">
        <nav class="cabecalho_menu">
            <a class="cabecalho_menu_link" href="index.html"> Home</a>
            <a class="cabecalho_menu_link" href="about.html">Sobre mim</a>
        </nav>
      </header>
      <main  class="apresentacao">
        <section class="apresentacao__conteudo">
            <h1 class="apresentacao__titulo"> Sobre mim</h1>
                <p class="apresentacao__conteudo__texto">
                    Olá! Sou Ryan, um desenvolvedor Front-end apaixonado por criar experiências digitais incríveis. Com 22 anos de idade e formado em Análise e Desenvolvimento de Sistemas pela UNIP, trago um conjunto sólido de habilidades e uma mentalidade inovadora para cada projeto que enfrento.
                    Minha jornada na UNIP me proporcionou uma compreensão abrangente das linguagens de programação, frameworks e ferramentas essenciais para o desenvolvimento web. Estou constantemente atualizado sobre as últimas tendências e técnicas no mundo do Front-end, buscando sempre superar expectativas e elevar a qualidade dos produtos que desenvolvo.
                </p>
                <p class="apresentacao__conteudo__texto">
                     Tenho um profundo entendimento das melhores práticas de design e usabilidade, o que me permite criar interfaces intuitivas e visualmente atraentes que cativam e envolvem os usuários. Além disso, sou colaborativo por natureza, trabalhando bem em equipe para transformar ideias em realidade.
                     Estou em busca de desafios estimulantes onde possa aplicar meu conhecimento e criatividade para construir soluções web excepcionais. 
                </p>
        </section>
        <img src="./assets/img2.png" alt="Foto de Perfil do Ryan">
      </main>
    <footer class="rodape">
    <p>Desenvolvido por Ryan Pelais.</p>
  </footer>
</body>
</html>

CSS

 @import url('https://fonts.googleapis.com/css2?family=Krona+One&family=Montserrat:wght@400;600&display=swap'); 

/** O procedimento acima esta importando uma fonte do google**/
:root{  /* o root server como um estoque de cores e fontes do projeto*/
    --cor-priamria: #000000;
    --cor-secundaria:#F6F6F6;   /**aqui esta nossa paleta de cores utilizada no projeto, caso você altere alguma cor nessa pelata ela sera aplicada a todos os lugares em que está sendo utilizada*/
    --cor-terciaria: #22d4fd;
    --cor-quartenario:#2385a3;

    --fonte-primaria:'krona one', 'sans-serif';     /* nessa parte está nossa paleta de fontes utilizadas no projeto*/
    --fonte-secundaria : 'Montserrat', 'sans-serif';
}

* { 
    margin: 0;    /** MARGIN SERVE PARA CONFIGURAR A O TAMANHO DA MARGEM DA PAGINA**/
    padding: 0;   /** SERVE PARA CONFIGURAR O ESPAÇAMENTO DA BORDA ATÉ O CONTEUDO **/   
}

body {
    /* height: 100vh; * ALTURA DA TELA, DEIXANDO 100% DA TELA DO NAVEGADOR* */
    box-sizing: border-box; /** SERVE PARA LIMITAR O ATE ONDE AS INFOMRÇÕES PODEM IR NA PAGINA PESQUISAR BOX SIZE MONZILA PARA TER REFERENCIA**/
    background: var(--cor-priamria); /**COR DO FUNDO DA PAGINA**/
    color: var(--cor-secundaria); /** COR DA LETRA DA PAGINA**/
}
.cabecalho{
    padding: 2% 0% 0% 15%;

}
.cabecalho_menu{    
    display: flex;
    gap: 80px;
}
.cabecalho_menu_link{
  font-family: var(--fonte-secundaria);
  font-size: 1.5rem;
  font-weight: 600;
  color:var(--cor-terciaria);
  text-decoration: none;
}

.apresentacao{
     display: flex;
     align-items: center; /*alinhamento do texto**/
     justify-content: space-between;
     padding: 4% 15%;
     
}

.apresentacao__conteudo{
    width: 615px;  /** PX SEGUINIFICA QUE VOCE QUER A CONFIGURAÇÃO EM PIXELS**/
    display: flex; /** posicionar elementos na tela**/
    flex-direction: column;
    gap: 40px;
}
.apresentacao__titulo{
    font-size: 2rem; /* 1 pixel igual a 16 rem, o rem server para as configurações de tamanho de fonte se aplique no seu projeto*/
    font-family: var(--fonte-primaria);
}
.titulo-destaque{   /**SERVE PARA CHAMAR A CLASSE ESPECIFICADA NA PAGINA HTML**/
    color:var(--cor-terciaria); /**COR DA LETRA DA CLASSE**/
}


.apresentacao__conteudo__texto{
    font-size: 1.40rem;
    font-family:var(--fonte-secundaria) ;
}
.apresentacao__links{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 32px;
    justify-content:space-between;
} 
.apresentacao_links_subtitulo{
    font-family: var(--fonte-primaria);
    font-size: 'Krona One','sans-serif';
    font-weight: 400;

}
.apresentacao__links__links{
    /* background-color: #22d4fd; */
    display: flex;
    justify-content: center;
    gap: 16px;
    border: 2px solid var(--cor-terciaria); /*Borda do botão*/
    width: 378px; /*espaçamento entre os botoes*/
    text-align: center;
    border-radius: 8px; /* formato da borda do botão*/
    font-size: 1.5rem;
    font-weight: 600;
    padding: 21.5px 0;  /*grossura do botão*/
    text-decoration: none;
    color: var(--cor-secundaria);
    font-family:  var(--fonte-secundaria);
    
}
/*Altera os botões quando passa o mouse em cima  :HOVER */
.apresentacao__links__links:hover{
    background-color: var(--cor-quartenario); /*muda a cor quando o mouse passa em cima*/
    padding: 3%; /*muda o tamanho quando o mouse passa*/
}
.rodape{
    color: var(--cor-priamria);
    background-color: var(--cor-terciaria);
    padding: 24px;
    text-align: center;
    font-family: var(--fonte-secundaria);
    font-size: 24;
    font-weight: 400px;

} 
