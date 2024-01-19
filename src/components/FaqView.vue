<template>
    <div class="faq_wrapper">
      <h1>Questions fréquemment posées:</h1>
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
          q: 'À qui est destiné cette application ?',
          a: 'Brogether est une application dédié à aider les EHPADS et plus particulièrement ses résidents. Elle également des prestataires afin de proposer des activités.',
          open: false
        },
        {
          q: 'Qu est-ce que cette application propose aux Ehpad et aux prestataires d activités ?',
          a: 'Notre application facilite la mise en relation entre les Ehpad et les prestataires d activités, offrant une plateforme conviviale pour planifier, coordonner et proposer une variété d activités et de services.',
          open: false
        },
        {
          q: 'Comment cette application garantit-elle la sécurité et la qualité des activités pour les résidents en Ehpad ?',
          a: 'Nous effectuons des vérifications rigoureuses des prestataires et proposons des fonctionnalités d évaluation et de rétroaction pour les Ehpad. Cela garantit que seules des activités de qualité sont proposées aux résidents, et que des mesures de sécurité sont mises en place pour préserver leur bien-être.',
          open: false
        },
        {
          q: 'Comment puis-je personnaliser les critères de sélection des prestataires d activités pour correspondre aux besoins spécifiques de notre Ehpad ?',
          a: 'Notre application offre des fonctionnalités avancées de filtrage et de personnalisation des critères de sélection des prestataires. Vous pouvez spécifier des préférences en fonction des types d activités, des horaires, de la localisation, et bien plus encore.',
          open: false
        },
        {
          q: 'Comment est gérée la communication entre les Ehpad et les prestataires d activités, notamment en cas de changements de planning ou d annulations ?',
          a: 'Nous avons un système de messagerie intégré qui permet une communication fluide entre les Ehpad et les prestataires. En cas de changements de planning ou d annulations, les deux parties sont notifiées instantanément.',
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
    max-width: 2000px;
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