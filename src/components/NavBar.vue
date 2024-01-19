<template>
    <v-app-bar app color="white" dark flat class="px-12" >
        <v-img src="logo.png" ></v-img>      
  
      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')" class="text-red">Accueil</v-btn>
      <v-btn text @click="scroll('about')"  >A Propos de Nous</v-btn>
      <v-btn text @click="scroll('portfolio')"  >Nos Etapes</v-btn>
      <v-btn text @click="scroll('services')" > Portfolio</v-btn>
      <v-btn text @click="scroll('page')"  > Notre Solution</v-btn>
      <v-btn text @click="scroll('biog')"  > Guide</v-btn>
      <v-btn text @click="scroll('contact')"  > Contact</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style>
  </style>