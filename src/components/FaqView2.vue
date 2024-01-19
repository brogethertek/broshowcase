<template>
    <div class="faq_wrapper">
      <h1>Guide d'utilisation:</h1>
      <div class="faq_field_wrapper">
        <div class="faq_field" v-for="(faq, i) in faqBase" :key="i">
          <div class="open-faq" @click="closeAllFaq(faq)">
            <h3>
              {{ faq.q }}
              <i class="fa-solid fa-plus" :class="faq.open ? 'rotate' : ''"></i>
            </h3>
            <p class="invisible" :class="faq.open ? 'visible' : ''">
              {{ faq.a }}
            </p> 
          </div>
        </div>
      </div>
    </div>
  </template>
  <script>
  import {ref} from 'vue'
  export default {
    setup() {
      const faqBase = ref([
        {
          q: 'Comment puis-je m inscrire en tant qu Ehpad ou prestataire d activités ?',
          a: 'L inscription est simple. Vous pouvez visiter notre site web ou télécharger l application, puis suivre les instructions pour créer un compte en tant qu Ehpad ou prestataire. Notre équipe est là pour vous aider à démarrer et répondre à vos questions.',
          open: false
        },
        {
          q: 'Comment puis-je en tant que responsable d un Ehpad rechercher des prestataires d activités disponibles ?',
          a: 'Vous pouvez utiliser la fonction de recherche de l application pour trouver des prestataires d activités dans votre région. Vous pouvez filtrer par type d activité, disponibilité, emplacement, etc.',
          open: false
        },
        {
          q: 'Puis-je suivre les évaluations et les retours des résidents sur les activités proposées ?',
          a: 'Oui, l application permet aux résidents de laisser des évaluations et des commentaires sur les activités. Vous pouvez consulter ces retours pour évaluer la satisfaction des résidents et améliorer votre sélection d activités.',
          open: false
        },
      ])
      const closeAllFaq = (item) => {
        if(!item.open) {
          faqBase.value.forEach(el => el.open = false)
        }
        item.open = !item.open;
      }
  
      return {faqBase, closeAllFaq}
    }
  }
  </script>
  <style scoped>
  
  .faq_wrapper {
    text-align: center;
    max-width: 1200px;
    margin: 40px auto;
  }
  
  .faq_field {
    border: 3px solid rgba(0, 0, 0, 0.624);
    border-radius: 10px;
    margin: 10px;
    background-color: rgba(255, 255, 255, 0.438);
  }
  
  .faq_field_wrapper {
    margin-top: 20px;
  }
  
  .invisible {
    visibility: hidden;
    opacity: 0;
    height: 0;
    transition: opacity .3s, height .3s, visibility .3s;
  }
  
  .visible {
    visibility: visible;
    height: 70px;
    opacity: 1;
    padding: 10px 20px;
  }
  
  .h3 {
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 18px 24px;
    margin: 8px 0;
  }
  
  .open_faq {
    cursor: pointer;
  }
  
  .rotate {
    transform: rotate(45deg);
  }
  
  .fa_plus {
    transition: transform 0.3s;
  }
  </style>