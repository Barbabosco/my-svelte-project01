<script>
  export let name;
</script>

<style>
  /*
blu scuro #013f8a
blu chiaro #026cbb

grigio scuro per i test #424245

*/

  * {
    margin: 0px;
    padding: 0px;
    /* outline: 1px solid red; */
    font-family: Oswald, Helvetica, sans-serif;
    text-decoration: none;
  }

  body {
  }

  .hamburger {
    position: absolute;
    top: 40px;
    right: 20px;
    cursor: pointer;
  }

  .headerContainer {
    width: 100%;
    background-color: #f2f2f2;
    border-bottom: 1px solid #e2e2e2;
  }

  .header {
    max-width: 1300px;
    /* background-color: aqua; */
    padding-right: 40px;
    padding-left: 40px;
    margin: auto;
    display: grid;
    grid-template-columns: 323px 1fr 300px;
    grid-template-rows: 130px;
    grid-gap: 0px;
  }

  .headerCell1 {
    align-self: center;
    /* height: 95px; */
  }

  .headerCell2 {
  }

  .headerCell3 {
    display: grid;
    grid-template-rows: 50% 50%;
    grid-template-columns: 300px;
    justify-items: stretch;
    /* align-items: stretch; */
  }

  .headerCell3Cell1 {
    background-color: #013f8a;
    text-align: center;
    display: grid;
    align-items: center;
  }

  .headerCell3Cell2 {
    background-color: #026cbb;
    text-align: center;
    display: grid;
    align-items: center;
  }

  @media (max-width: 700px) {
    .header {
      grid-template-rows: 110px;
    }

    .headerCell3Cell1,
    .headerCell3Cell2 {
      display: none;
    }
  }

  @media (min-width: 701px) {
    .hamburger {
      display: none;
    }
  }

  @media (max-width: 450px) {
    .headerLogo {
      max-width: 280px;
    }
  }

  @media (max-width: 400px) {
    .header {
      grid-template-rows: 80px;
    }
    .headerLogo {
      max-width: 240px;
    }
    .hamburger {
      top: 20px;
    }
  }

  @media (max-width: 350px) {
    .header {
      grid-template-rows: 70px;
    }
    .headerLogo {
      max-width: 190px;
    }
  }

  @media (max-width: 300px) {
    .header {
      grid-template-rows: 60px;
    }
    .headerLogo {
      max-width: 130px;
    }
  }

  .headerLink {
    color: white;
    font-weight: 300;
    font-size: 1.6rem;
    text-transform: uppercase;
    text-decoration: none;
  }

  .navContainer {
    width: 100%;

    border-bottom: 1px solid #e2e2e2;
  }

  nav {
    max-width: 1300px;
    padding-right: 40px;
    padding-left: 40px;
    margin: auto;
    height: 75px;
    display: flex;
    align-items: flex-start;
  }

  @media (max-width: 700px) {
    nav {
      display: none;
    }
  }
  .navItem {
    color: #013f8a;
    margin-right: 50px;
    height: 75px;
    /* background-color: yellow; */
    display: flex;
    align-items: center;
  }

  .navItemSelected {
    border-top: 2px solid #013f8a;
    margin-top: -1px;
  }

  .navItemInside {
    font-weight: 400;
    font-size: 1.3rem;
  }

  @media (max-width: 1200px) {
    .navItem {
      margin-right: 40px;
    }
    .navItemInside {
      font-size: 1.1rem;
    }
  }

  @media (max-width: 1000px) {
    .navItem {
      margin-right: 30px;
    }
    .navItemInside {
      font-size: 1rem;
    }
  }

  @media (max-width: 800px) {
    .navItem {
      margin-right: 20px;
    }
    .navItemInside {
      font-size: 0.85rem;
    }
  }

  .navLink,
  .navLink:link,
  .navLink:visited,
  .navLink:active,
  .navLink:hover {
    text-transform: uppercase;
    text-decoration: none;
    color: #013f8a;
  }

  .crumbsContainer {
    width: 100%;
    height: 85px;
  }

  .crumbs {
    max-width: 1300px;
    padding-right: 40px;
    padding-left: 40px;
    margin: auto;
    padding-right: 40px;
    padding-left: 40px;
    height: 85px;
    display: flex;
    align-items: center;
    color: #444444;
    font-size: 1.1rem;
  }
  .crumbsLink,
  .crumbsLink:link,
  .crumbsLink:visited,
  .crumbsLink:active,
  .crumbsLink:hover {
    text-decoration: none;
    color: #013f8a;
  }
  .homeGridContainer {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 30px;
  }
  .homeGridCell,
  .homeGridCell:link,
  .homeGridCell:visited,
  .homeGridCell:active,
  .homeGridCell:hover {
    min-height: 350px;
    color: white;
    text-align: center;
    padding-top: 40px;
    text-decoration: none;
    background-position: center center;
    background-repeat: no-repeat;
  }
  .homeGridCellOdd {
    background-color: #013f8a;
  }
  .homeGridCellEven {
    background-color: #026cbb;
  }

  .homeGridCell1 {
    background-image: url("../images/ambiente.jpg");
  }
  .homeGridCell2 {
    background-image: url("../images/sicurezza.jpg");
  }
  .homeGridCell3 {
    background-image: url("../images/gestione.jpg");
  }
  .homeGridCell4 {
    background-image: url("../images/medicina.jpg");
  }
  .homeGridCell5 {
    background-image: url("../images/formazione.jpg");
  }
  .homeGridCell6 {
    background-image: url("../images/edilizia.jpg");
  }

  .homeH1 {
    text-transform: uppercase;
    font-size: 2rem;
    font-weight: 400;
  }

  .homeP {
    padding-top: 20px;
    font-size: 1.2rem;
    font-weight: 400;
    margin-right: 10%;
    margin-left: 10%;
  }

  @media (max-width: 800px) {
    .homeGridContainer {
      grid-template-columns: 1fr 1fr;
      grid-gap: 20px;
    }
  }
  @media (max-width: 550px) {
    .homeGridContainer {
      grid-template-columns: 1fr;
      /* grid-gap: 10px; */
    }
  }
  .overFooterContainer {
    width: 100%;
    height: 40px;
  }

  .homeOverFooterContainer {
    width: 100%;
    height: 85px;
  }

  .footerContainer {
    background-color: lightblue;
    width: 100%;
  }

  footer {
    display: grid;
    background-color: #f2f2f2;
    grid-template-columns: 3fr 1fr;
    padding-right: 40px;
    padding-left: 40px;
  }

  .footerCell1 {
    padding-top: 50px;
    padding-bottom: 50px;
    color: #424245;
    font-size: 1.1rem;
  }

  .footerCell2 {
    padding-top: 50px;
    padding-bottom: 50px;
    color: #424245;
    justify-self: end;
  }

  .footerLink,
  .footerLink:link,
  .footerLink:visited,
  .footerLink:active,
  .footerLink:hover {
    text-decoration: underline;
    color: #424245;
    font-size: 1.1rem;
  }

  .footerTitle {
    color: #013f8a;
    font-weight: 700;
    font-size: 1.1rem;
    line-height: 4rem;
  }

  @media (max-width: 700px) {
    footer {
      grid-template-columns: 1fr;
      /* grid-gap: 20px; */
    }
    .footerCell2 {
      justify-self: start;
    }
  }

  .underFooterContainer {
    width: 100%;
    height: 85px;
    padding-top: 20px;
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 0.8rem;
    color: #888888;
  }

  .kLink,
  .kLink:link,
  .kLink:visited,
  .kLink:active,
  .kLink:hover {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 0.8rem;
    color: #888888;
    text-decoration: underline;
  }

  .mobiMenu {
    width: 100%;
    height: 200px;
    position: absolute;
    display: none;
    grid-template-columns: 1fr;
    align-items: stretch;
    top: 110px;
    left: 0px;
    background-color: #f2f2f2;
    border-top: 2px solid #e2e2e2;
    border-bottom: 2px solid #e2e2e2;
    align-items: stretch;
  }
  .mobiMenuCell {
    background-color: #f2f2f2;
    padding-left: 40px;
    height: 45px;
    border-bottom: 1px solid #e2e2e2;
    display: grid;
    align-items: center;
  }

  .mobiMenuCellInside {
    background-color: orange;
  }

  .mobiMenuCellColor {
    background-color: yellow;
  }
  .mobiMenuLink,
  .mobiMenuLink:link,
  .mobiMenuLink:visited,
  .mobiMenuLink:active,
  .mobiMenuLink:hover {
    text-transform: uppercase;
    color: #013f8a;
    font-size: 1.1rem;
  }

  .alertContainer {
    position: fixed;
    background-color: #fee700;
    width: 100%;
    /* height: 200px; */
    bottom: 0px;
    display: block;
  }

  .alert {
    max-width: 1300px;
    /* padding-right: 40px;
  padding-left: 40px; */
    padding: 40px;
    margin: auto;
    display: grid;
    grid-template-columns: 8fr 1fr;
    grid-template-rows: auto;
    column-gap: 20px;
  }

  .alertCell1 {
    justify-self: end;
    grid-area: 1/1/2/2;
  }

  .alertCell2 {
    justify-self: end;
    grid-area: 1/2/2/3;
  }

  .alertTitle {
    color: #000000;
    font-size: 24px;
    font-weight: 700;
  }

  .alertClose {
    cursor: pointer;
  }

  .alertP {
    font-size: 1rem;
    line-height: 1.2rem;
  }

  @media (max-width: 801px) {
    .alertContainer {
      /* grid-template-columns: auto;
    grid-template-rows: auto auto; */
      display: none;
    }
  }

  .mainContainer {
    width: 100%;
  }

  .main {
    max-width: 1300px;
    padding-right: 40px;
    padding-left: 40px;
    margin: auto;
  }

  .mainTwo {
    display: grid;
    grid-template-columns: 50% 50%;
    grid-gap: 40px;
  }

  .h1Internal {
    color: #013f8a;
    font-size: 2rem;
    text-transform: uppercase;
  }

  .mainTwoCell {
    margin-top: 30px;
  }

  p {
    font-size: 1.2rem;
    font-weight: 400;
    line-height: 2.2rem;
    margin-top: 0.75rem;
  }

  @media (max-width: 801px) {
    .mainTwo {
      display: block;
    }
  }

  .mainOne {
    /* background-color: chartreuse; */
  }

  .h2Internal {
    color: #424245;
    font-size: 1.4rem;
  }

  .h2InternalLink,
  .h2InternalLink:link,
  .h2InternalLink:visited,
  .h2InternalLink:active,
  .h2InternalLink:hover {
    color: #013f8a;
    text-decoration: underline;
  }

  .ulAttivita {
    margin: 20px 50px;
  }

  .liAttivita {
    color: #424245;
    font-size: 1.2rem;
    font-weight: 500;
  }

  .h3Internal {
    color: #013f8a;
    font-size: 1.4rem;
    margin-top: 30px;
  }

  .h2Alert {
    color: #424245;
    font-size: 1.4rem;
    background-color: #fee700;
    padding: 10px;
  }

  .h2AlertLink,
  .h2AlertLink:link,
  .h2AlertLink:visited,
  .h2AlertLink:active,
  .h2AlertLink:hover {
    color: #013f8a;
    text-decoration: underline;
  }
</style>

<img src="./images/hamburger.jpg" class="hamburger" />
<section class="headerContainer">
  <div class="header">
    <div class="headerCell1">
      <img src="images/logo-studiovicentin.jpg" class="headerLogo" />
    </div>
    <div class="headerCell2" />
    <div class="headerCell3">
      <div class="headerCell3Cell1">
        <div>
          <a class="headerLink" href="tel:+390444400877">+39 0444 400 877</a>
        </div>
      </div>
      <div class="headerCell3Cell2">
        <div>
          <a
            class="headerLink"
            href="mailto=studio@studiovicentin.it"
            target="_blank">studio@studiovicentin.it</a>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="navContainer">
  <nav>
    <div class="navItem navItemSelected">
      <div class="navItemInside">
        <a href="index.html" class="navLink">homepage</a>
      </div>
    </div>
    <div class="navItem">
      <div class="navItemInside">
        <a href="studio.html" class="navLink">Lo studio</a>
      </div>
    </div>
    <div class="navItem">
      <div class="navItemInside">
        <a href="attivita.html" class="navLink">Attività</a>
      </div>
    </div>
    <div class="navItem">
      <div class="navItemInside">
        <a href="news.html" class="navLink">news</a>
      </div>
    </div>
    <!-- <div class="navItem">
			<div class="navItemInside">
				<a href="approfondimenti.html" class="navLink">approfondimenti</a>
			</div>
		</div> -->
    <div class="navItem">
      <div class="navItemInside">
        <a href="corsi.html" class="navLink">corsi</a>
      </div>
    </div>
    <div class="navItem">
      <div class="navItemInside">
        <a href="contatti.html" class="navLink">contatti e sede</a>
      </div>
    </div>
  </nav>
</section>

<section class="homeGridContainer">
  <a href="ambiente.html">
    <div class="homeGridCell homeGridCellOdd homeGridCell1">
      <h1 class="homeH1">Ambiente</h1>
      <p class="homeP">
        Servizio integrato di consulenza, progettazione ed assistenza tecnica
        per la gestione degli adempimenti ambientali.
      </p>
    </div>
  </a>

  <a href="sicurezza.html">
    <div class="homeGridCell homeGridCellEven homeGridCell2">
      <h1 class="homeH1">Sicurezza e Prevenzione</h1>
      <p class="homeP">
        Servizio completo di consulenza ed assistenza per la gestione degli
        adempimenti in materia di sicurezza e salute nel lavoro.
      </p>
    </div>
  </a>

  <a href="gestione.html">
    <div class="homeGridCell homeGridCellOdd homeGridCell3">
      <h1 class="homeH1">Sistemi di gestione</h1>
      <p class="homeP">
        Consulenza ed assistenza tecnica per integrazione e mantenimento nel
        tempo di Sistemi di Gestione Aziendale.
      </p>
    </div>
  </a>

  <a href="medicina.html">
    <div class="homeGridCell homeGridCellEven homeGridCell4">
      <h1 class="homeH1">Medicina del lavoro</h1>
      <p class="homeP">
        Incarico di Medico Competente per l’Azienda, nomina formale ed
        elaborazione del Protocollo Sanitario, sorveglianza sanitaria.
      </p>
    </div>
  </a>

  <a href="formazione.html">
    <div class="homeGridCell homeGridCellOdd homeGridCell5">
      <h1 class="homeH1">Formazione</h1>
      <p class="homeP">
        Lo studio organizza Corsi di Formazione per le principali tematiche in
        Materia di Sicurezza sul lavoro.
      </p>
    </div>
  </a>

  <a href="edilizia.html">
    <div class="homeGridCell homeGridCellEven homeGridCell6">
      <h1 class="homeH1">Edilizia e urbanistica</h1>
      <p class="homeP">
        Servizio completo ed integrato di consulenza, progettazione, direzione
        lavori ed assistenza tecnica ad Aziende e Privati.
      </p>
    </div>
  </a>
</section>

<section class="homeOverFooterContainer" />
<section class="footerContainer">
  <footer>
    <div class="footerCell1">
      <span class="footerTitle">Studio Vicentin s.r.l.</span>
      <p>
        P.IVA 03852890247<br />
        Via Alcide De Gasperi, 26 36040 Brendola (Vicenza)<br />
        Tel:
        <a href="tel:0444400877" class="footerLink">0444 400877</a>
        -
        <a href="tel:0444400647" class="footerLink">400647</a>
        - Fax: 0444 405210<br />
        Mail:
        <a
          href="mailto:studio@studiovicentin.it"
          class="footerLink">studio@studiovicentin.it</a>
      </p>
    </div>
    <div class="footerCell2">
      <a
        href="https://www.iubenda.com/privacy-policy/7969219"
        class="footerLink"
        target="_blank"
        rel="noopener">Privacy policy</a>
      -
      <a
        href="https://www.iubenda.com/privacy-policy/7969219/cookie-policy"
        class="footerLink"
        target="_blank"
        rel="noopener">Cookie policy</a>
    </div>
  </footer>
</section>
<section class="underFooterContainer">
  Made in
  <a
    href="https://www.antartika.it"
    class="kLink"
    target="_blank"
    rel="noopener">Antartika</a>
</section>

<div class="mobiMenu">
  <div class="mobiMenuCell">
    <a href="index.html" class="mobiMenuLink">Homepage</a>
  </div>
  <div class="mobiMenuCell">
    <a href="studio.html" class="mobiMenuLink">studio</a>
  </div>
  <div class="mobiMenuCell">
    <a href="attivita.html" class="mobiMenuLink">Attività</a>
  </div>
  <div class="mobiMenuCell">
    <a href="news.html" class="mobiMenuLink">news</a>
  </div>
  <div class="mobiMenuCell">
    <a href="approfondimenti.html" class="mobiMenuLink">approfondimenti</a>
  </div>
  <div class="mobiMenuCell">
    <a href="corsi.html" class="mobiMenuLink">Corsi</a>
  </div>
  <div class="mobiMenuCell">
    <a href="contatti.html" class="mobiMenuLink">Contatti e sede</a>
  </div>
</div>
