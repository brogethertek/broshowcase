<template>
    <v-app id="home">
      <NavBar />
      <v-container fluid>
        <div class="head">
          <v-row>
            <v-col cols="5">
              <div style="position: relative" class="mt-16">
                <h1 class="text-white">Salut,</h1>
                <h1 class="text-white">Nous sommes Brogether</h1>
                <span class="text-white">Renous le lien, brisons la solitude</span><br />
              </div>
            </v-col>
            <v-col cols="2">
              <div
                style="
                  position: absolute;
                  z-index: 9999;
                  bottom: 0;
                  margin-left: auto;
                  margin-right: auto;
                  left: 0;
                  right: 0;
                  text-align: center;
                "
                class="mt-16"
              >
                <v-icon>fas fa-angle-double-down</v-icon>
              </div>
            </v-col>
            <v-col cols="5">
              <div style="position: relative; z-index: 9999" class="mt-16">
                <v-img src="logo.png" contain max-height="300"></v-img>
              </div>
            </v-col>
          </v-row>
        </div>
        <v-col cols="12" class="mt-16" id="about">
          <div>
            <v-row>
              <v-col cols="12" sm="6">
                <div class="egg">
                  <v-img src="epi.png" max-height="200" class=""></v-img>
                </div>
              </v-col>
              <v-col cols="12" sm="6">
                <h5 class="mt-16">A propos de nous</h5>
                <div style="width: 120px">
                  <v-slider
                    v-model="slider2"
                    color="#D35D56"
                    label="track-color"
                  ></v-slider>
                </div>
                <h4 class="mt-n4">Nous sommes des étudiants d'EPITECH</h4>
                <p class="text-grey">
                  Dans le cadre de notre projet de fin d'études nous deviosn répondre à un problème 
                  et trouver une solution digitale à celle-ci. Nous avons donc décider d'aider et 
                  essayer de répondre à la porblématique de la misère sociale dans les EHPAD.
                </p>
                <br />
                <p class="text-grey">
                  C'est un projet très ambitieux mais qui nous tiens à coeur.
                  Dans ce porjet nous sommes une équipe de 6 étudiants qui travaillont en développement 
                  informatique. Nous avons donc trouver comme solution la mise en place d'une application 
                  web et mobile qui met en lien les EHPAD et des prestataires proposant de activités afin 
                  de divertir et d'oocuper les journées de nos seniors.
                </p>
                <br />
                <br />
                <h4 class="mt-n4">Voici qui nous sommes :</h4>
                <br />
                <br />
                <div class="flip">
                  <div class="front"></div>
                  <h3>David Sokhan Sanj</h3>
                  <div class="back">
                    <h3>Frontend Web</h3>
                    <p>
                      Développement en Vue.js et travail surtout sur le design et 
                      l'utilisation du back-end.
                    </p>
                  </div>
                </div>
                <div class="flip3">
                  <div class="front3"></div>
                  <h3>Merlin Jallu</h3>
                  <div class="back3">
                    <h3>Frontend Mobile</h3>
                    <p>
                      Développement en React Native. 
                      Travail sur la partie entreprise/prestataires au niveau de la création et rendu final.
                    </p>
                  </div>
                </div>
                <div class="flip4">
                  <div class="front4"></div>
                  <h3>Pablo Etienne</h3>
                  <div class="back4">
                    <h3>Frontend Web</h3>
                    <p>
                      Développement en Vue.js et travail sur le fonctionnel, et plus précisement sur l'aspect utilisateur côté EHPAD.
                    </p>
                  </div>
                </div>
                <div class="flip5">
                  <div class="front5"></div>
                  <h3>Enzo Ekobo</h3>
                  <div class="back5">
                    <h3>Backend</h3>
                    <p>Developpement et création des routes côté Backend. Développement en node JS.</p>
                  </div>
                </div>
                <div class="flip6">
                  <div class="front6"></div>
                  <h3>Alexandre Descoins</h3>
                  <div class="back6">
                    <h3>Backend</h3>
                    <p>
                      Création d'une API pour la gestion des activités/ressources, 
                      et sur la sécurisation du backend sous
                      node JS.
                    </p>
                  </div>
                </div>
                <div class="flip7">
                  <div class="front7"></div>
                  <h3>Xavier Pain</h3>
                  <div class="back7">
                    <h3>Devops</h3>
                    <p>DevOps Optimisation & Automatisation de l'infrastructure.</p>
                  </div>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col cols="12" class="padd" id="portfolio">
          <div class="text-center mt-4">
            <h2>Le Parcours</h2>
            <div style="width: 120px; margin: 0 auto">
              <v-slider
                v-model="slider2"
                color="#D35D56"
                label="track-color"
              ></v-slider>
            </div>
          </div>
          <div class="first" id="project">
            <v-row>
              <v-col cols="12">
                <div class="child">
                  <v-btn
                    icon="fas fa-book"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Test & Learn</h3>
                  <h4 class="ml-3 mt-4">Avril 2022 - Juin 2022</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    Ce premier sprint de trois mois a pour but de nous placer<br />
                    dans une situation où nous devons développer notre projet<br />
                    en suivant une organisation, en essayant diverses <br />
                    méthodologies, méthodes d’organisations internes, <br />
                    et moyens de communications, afin que nous trouvion <br />
                    ce qui nous convient le mieux et nous permet d’être <br />
                    les plus productifs possibles. Comme indiqué par le <br />
                    nom du sprint, il s’agit donc de tester, et d’en tirer les leçons.
                    
                  </p>
                </div>
                <div class="child">
                  <v-btn
                    icon="fas fa-mobile-alt"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Management & Process</h3>
                  <h4 class="ml-3 mt-4">Juillet 2022 - Octobre 2022</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    Forts de notre expérimentation lors du sprint précédent, <br />
                    l’objectif de celui-ci était de véritablement structurer et pérenniser <br />
                    l’organisation que nous avions mis en place.
                    <br /><br /><br /><br /><br /><br />
                  </p>
                </div>
                <div class="child">
                  <v-btn
                    icon="fas fa-camera"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Fast Forward</h3>
                  <h4 class="ml-3 mt-4">Novembre 2022 - Janvier 2023</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    L’objectif de ce troisième sprint,  <br />
                    d’une durée de trois mois, est d’avoir une avancée  <br />
                    significative dans le développement <br />
                    de notre projet. Lors des sprints précédents, nous avons eu <br />
                    l’occasion d’expérimenter autour  <br />
                    de notre projet et de sa gestion, <br />
                    ainsi que de structurer cela afin de créer des automatismes et <br />
                    des méthodes saines de fonctionnement entre nous.
                  </p>
                </div>
              </v-col>
            </v-row>
            <v-divider></v-divider>
          </div>
  
          <div class="first" id="project">
            <v-row>
              <v-col cols="12">
                <div class="child">
                  <v-btn
                    icon="fas fa-laptop"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Beta & Growth Hacking</h3>
                  <h4 class="ml-3 mt-4">Février 2023 - Mai 2023</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    Suite au sprint Fast Forward, nous avons eu une <br />
                    avancée notable sur notre projet, qui a nous à <br />
                    permis de pouvoir envisager de communiquer <br />
                    sérieusement auprès des utilisateurs cibles de notre projet. <br />
                    L’objectif de ce sprint de quatre mois est <br />
                    donc de faire de l’acquisition utilisateur <br />
                    en vue de lancer notre bêta au mois de mai 2023. <br />
                    Cette bêta doit être cohérente avec l’avancement <br />
                    de notre projet à cette période, nous devons donc <br />
                    choisir entre une bêta publique ou une bêta privée <br />
                    en fonction de cela.Suite au sprint Fast Forward, <br />
                    nous avons eu une avancée notable sur notre projet, <br />
                    qui a nous à permis de pouvoir envisager de communiquer <br />
                    sérieusement auprès des utilisateurs cibles de notre projet. <br />
                    L’objectif de ce sprint de quatre mois est donc de <br />
                    faire de l’acquisition utilisateur en vue de lancer <br />
                    notre bêta au mois de mai 2023. Cette bêta doit être <br />
                    cohérente avec l’avancement de notre projet à <br />
                    cette période, nous devons donc choisir entre une <br />
                    bêta publique ou une bêta privée en fonction de cela.
                  </p>
                </div>
                <div class="child">
                  <v-btn
                    icon="fas fa-house"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Consolidation</h3>
                  <h4 class="ml-3 mt-4">Juin 2023 - Septembre 2023</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    Au sprint précédent, nous avons acquis des utilisateurs, <br />
                    et notre bêta a été lancée. Il est donc désormais temps <br />
                    d’écouter nos utilisateurs et de prendre en compte <br />
                    leurs retours.<br />
                    <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
                  </p>
                </div>
                <div class="child">
                  <v-btn
                    icon="fas fa-mobile-alt"
                    color="#5892C3"
                    class="text-white"
                  ></v-btn>
                  <h3 class="ml-3 mt-4">Launch & Metrics</h3>
                  <h4 class="ml-3 mt-4">Octobre 2023 - Décembre 2023</h4>
                  <p class="text-grey ml-3 mt-4 text-caption">
                    bêta, recruté des utilisateurs, avons étudié leur <br />
                    comportement et avons pris en compte leurs retours. <br />
                    Il est donc désormais temps de lancer, à proprement <br />
                    parler, notre projet et de mettre en place les outils <br />
                    nécessaires au suivi d’un projet en production.<br />
                    <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
                  </p>
                </div>
              </v-col>
            </v-row>
            <v-divider></v-divider>
          </div>
          <br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
        </v-col>
        <v-col cols="12" sm="12" id="services">
          <div class="text-center mt-4">
            <h2>Portfolio</h2>
            <div style="width: 120px; margin: 0 auto">
              <v-slider
                v-model="slider2"
                color="#D35D56"
                label="track-color"
              ></v-slider>
            </div>
          </div>
          <div class="d-flex justify-center mb-6">
            <v-btn color="#5892C3" class="mr-2">Tous</v-btn>
            <v-btn class="mr-2" variant="tonal">Activités</v-btn>
            <v-btn class="mr-2" variant="tonal">EHPAD</v-btn>
            <v-btn class="mr-2" variant="tonal"> Presatatires</v-btn>
            <v-btn variant="tonal"> Retours</v-btn>
          </div>
        </v-col>
        <v-col cols="12" class="imgHover">
          <v-row class="fill-height" align="center" justify="center">
            <template v-for="(item, i) in items" :key="i">
              <v-col cols="12" md="4">
                <v-hover v-slot="{ isHovering, props }">
                  <v-card
                    :elevation="isHovering ? 12 : 2"
                    :class="{ 'on-hover': isHovering }"
                    v-bind="props"
                  >
                    <v-img :src="item.img" height="225px" cover> </v-img>
                  </v-card>
                </v-hover>
              </v-col>
            </template>
          </v-row>
        </v-col>
        <v-col cols="12" sm="12">
          <div class="d-flex justify-center mb-6">
            <v-btn color="#5892C3" class="mt-4">Plus</v-btn>
          </div>
        </v-col>
        <br /><br /><br /><br /><br /><br />
        <v-col cols="12" id="page">
          <div class="text-center mt-4">
            <h2>Pourquoi ?</h2>
            <div style="width: 120px; margin: 0 auto">
              <v-slider
                v-model="slider2"
                color="#D35D56"
                label="track-color"
              ></v-slider>
            </div>
          </div>
          <div class="pre">
            <v-row>
              <v-col cols="12" sm="4">
                <v-card class="mx-auto" max-width="344" height="">
                  <v-img src="equipe.JPG" height="200px" cover></v-img>
  
                  <v-card-title> Présentation du Projet </v-card-title>
                  <v-card-text>
                    Notre application est une plateforme de mise en relation entre des EHPAD et des particuliers ou des entreprises proposant des activités adaptées aux seniors. L'objectif est de favoriser le bien-être et la socialisation des résidents en proposant une grande variété d'activités, allant de la musique à la gymnastique douce en passant par des ateliers créatifs. Les particuliers et les entreprises peuvent facilement proposer leurs services et les EHPAD peuvent trouver des activités sur mesure pour leurs résidents. Notre application est simple d'utilisation et permet de mettre en relation les différents acteurs en quelques clics. Nous sommes convaincus que notre application contribuera à améliorer la qualité de vie des personnes âgées et à favoriser leur épanouissement au sein des EHPAD.
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4">
                <v-card class="mx-auto" max-width="344" height="">
                  <v-img src="presta.jpeg" height="200px" cover></v-img>
  
                  <v-card-title> Prestataires </v-card-title>
                  <v-card-text>
                    Vous voulez agrandir votre public aux seniors ? Vous êtes désireux de partager votre savoir-faire de l'amusement et de l'épanouissement a un public trop souvent mis de côté ? Vous êtes désireux de devenir une référence au prêt de nombreuses structures ? Alors brogether est fait pour vous ! Crée votre profil et rentrez en contact avec tous nos membres.
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="12" sm="4">
                <v-card class="mx-auto" max-width="344" height="">
                  <v-img src="retraite.jpg" height="200px" cover></v-img>
  
                  <v-card-title> EHPAD </v-card-title>
                  <v-card-text>
                    Votre EHPAD est désireuse d'amener joie, amusement et épanouissement a son public ? Vous voulez avoir accès à un panel d'activités divers et varier tout en arrêtant de devoir faire des heures de recherches ? Alors il n'y a plus qu'un pas à faire, votre profil sur BROGHER afin d'avoir accès aux nombreux partenaires désireux de vous proposer des nombreuses activités diverses varie et adapté au bien-être de votre public !
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <br /><br /><br /><br />
        <v-col cols="12" id="biog">
          <div class="hire">
            <v-row>
              <v-col cols="12" sm="8">
                <h1 class="mt-9">Comment utiliser notre applictaion</h1>
                <p class="text-grey">
                  Voici une FAQ ainsi qu'un guide d'utilisation de notre application afin de vous 
                  y retrouver facilelement si vous décider de l'utiliser.
                </p>
              </v-col>
              <!--<v-col cols="12" sm="4">
                <v-btn color="#FBDF7E" class="mt-15">Guide</v-btn>
              </v-col>-->
            </v-row>
            <FaqView />
            <FaqView2 />
          </div>
        </v-col>
        <br /><br />
        <v-col cols="12" sm="12" class="px-16" id="contact">
          <v-row>
            <v-col cols="12" sm="4">
              <div class="child">
                <h1>Informations</h1>
                <v-btn
                  icon="fas fa-map-marker-alt"
                  color=""
                  class="mt-10"
                  variant="outlined"
                ></v-btn
                ><br />
                <span class="text-caption">Ecole informatique Paris - Epitech<br />
                  14-16 Rue Voltaire, 94270 Le Kremlin-Bicêtre </span
                ><br />
                <v-btn
                  icon="fas fa-phone-alt"
                  color=""
                  class="mt-10"
                  variant="outlined"
                ></v-btn
                ><br />
                <span class="text-caption">+330000000 </span> <br />
                <v-btn
                  icon="fas fa-envelope"
                  color=""
                  class="mt-10"
                  variant="outlined"
                ></v-btn
                ><br />
                <span class="text-caption">brogether24.pro@gmail.com </span> <br />
                <span class="text-caption">brogether_2024@labeip.epitech.eu </span> <br />
              </div>
            </v-col>
            <v-col cols="12" sm="8">
              <h1 class="mt-8">Envoyer un message</h1>
              <v-divider></v-divider>
              <span class="text-caption"
                >Vous avez encore des questions ou des renseignements que vous n'avez pas eu ? Pas de soucis, envoyez nous des à présent un mail et nous tâcherons d'y répondre le plus brièvement possible !</span
              >
              <v-row class="mt-10">
                <v-col cols="12" sm="6">
                  <v-text-field
                    label="Nom"
                    persistent-hint
                    variant="outlined"
                  ></v-text-field>
                </v-col>
                <v-col cols="12" sm="6">
                  <v-text-field
                    label="Numéro de Téléphone"
                    persistent-hint
                    variant="outlined"
                  ></v-text-field>
                </v-col>
              </v-row>
              <v-textarea
                label="Message"
                persistent-hint
                variant="outlined"
              ></v-textarea>
              <v-btn color="#5892C3" class="mt-2">Envoyer</v-btn>
            </v-col>
          </v-row>
        </v-col>
      </v-container>
      <FooterView />
    </v-app>
  </template>
  
  <script>
  import { defineComponent } from "vue";
  import NavBar from "../components/NavBar.vue";
  import FooterView from "../components/FooterView.vue";
  import FaqView from "../components/FaqView.vue";
  import FaqView2 from "../components/FaqView2.vue";
  
  export default defineComponent({
    name: "HomeView",
    setup() {
      return {
        slider2: 50,
  
        items: [
          {
            img: "ehpad1.jpg",
          },
          {
            img: "peinture.jpg",
          },
          {
            img: "magie.jpg",
          },
          {
            img: "ehpad3.jpg",
          },
          {
            img: "danse.jpg",
          },
          {
            img: "ehpad4.jpg",
          },
        ],
      };
    },
    components: {
      NavBar,
      FooterView,
      FaqView,
      FaqView2
  },
  });
  </script>
  <style scoped>
  .v-container {
    padding: 16px 0 16px 0;
  }
  
  .head {
    position: relative;
    text-align: center;
    padding: 12px;
    margin-bottom: 6px;
    height: 400px;
    width: 100%;
    color: white;
  }
  .head:before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 50%;
    background: rgb(139, 139, 139);
    transform: skew(0deg, 6deg);
  }
  .head:after {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    height: 100%;
    width: 50%;
    background: rgb(139, 139, 139);
    transform: skew(0deg, -6deg);
  }
  .egg {
    display: block;
    margin-left: 100px;
    margin-top: 50px;
    width: 356px;
    height: 300px;
    background-color: #5892C3;
    border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
  }
  .first {
    width: 100%;
    height: 350px;
    text-align: center;
    padding: 2rem 2rem;
  }
  .child {
    display: inline-block;
    padding: 2rem 1rem;
    vertical-align: middle;
    text-align: center;
    margin-right: 8px;
  }
  
  .imgHover {
    padding: 0 200px;
  }
  .pre {
    width: 100%;
    height: 750px;
    text-align: center;
    padding: 0 200px;
    background-color: #f5f5f5;
  }
  .hire {
    width: 100%;
    height: 1000px;
    padding: 0 200px;
    background-color: #e9e9e9;
    margin-top: -24px;
  }
  
  .flip {
      position: relative;
      top: 0%;
      left: -600Px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front,.back {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front {
      background-image: url("../../public/dav.jpg");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip:hover .front {
      transform: rotateY(180deg);
  }
  
  .flip:hover .back {
      opacity: 1;
      transform: rotateY(0);
  }
  
  
  .flip3 {
      position: relative;
      top: -200px;
      left: -400px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front3,.back3 {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front3 {
      background-image: url("../../public/Merlin.jpg");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back3 {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip3:hover .front3 {
      transform: rotateY(180deg);
  }
  
  .flip3:hover .back3 {
      opacity: 1;
      transform: rotateY(0);
  }
  
  .flip4 {
      position: relative;
      top: -400px;
      left: -200px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front4,.back4 {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front4 {
      background-image: url("../../public/pablo.jpg");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back4 {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip4:hover .front4 {
      transform: rotateY(180deg);
  }
  
  .flip4:hover .back4 {
      opacity: 1;
      transform: rotateY(0);
  }
  
  .flip5 {
      position: relative;
      top: -600px;
      left: 0px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front5,.back5 {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front5 {
      background-image: url("../../public/enzo.jpeg");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back5 {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip5:hover .front5 {
      transform: rotateY(180deg);
  }
  
  .flip5:hover .back5 {
      opacity: 1;
      transform: rotateY(0);
  }
  
  .flip6 {
      position: relative;
      top: -800px;
      left: 200px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front6,.back6 {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front6 {
      background-image: url("../../public/Alex.jpg");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back6 {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip6:hover .front6 {
      transform: rotateY(180deg);
  }
  
  .flip6:hover .back6 {
      opacity: 1;
      transform: rotateY(0);
  }
  
  .flip7 {
      position: relative;
      top: -1000px;
      left: 400px;
      height: 200px;
      width: 200px;
      text-align: center;
  }
  
  .front7,.back7 {
      background-color: #a7a6a5d1;
      display: block;
      width: 175px;
      height: 175px;
      border-radius: 10px;
      transition: all .5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  
  .front7 {
      background-image: url("../../public/xavier.png");
      background-position: center;
      background-size: cover;
      box-shadow: 0 5px 20px rgba(255, 255, 255, 0.205);
      transform: rotateY(0);
  }
  
  .back7 {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 10px;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      transform: rotateY(-180deg);
  }
  
  .flip7:hover .front7 {
      transform: rotateY(180deg);
  }
  
  .flip7:hover .back7 {
      opacity: 1;
      transform: rotateY(0);
  }
  </style>
  