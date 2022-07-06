<!-- Descrizione:
Create un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone. -->


<template>
  <div id="app">
    <MyHeader/>

    <main>
      <SectionMainContent/>
    </main>
  </div>
</template>


<script>
import MyHeader from './components/MyHeader.vue';
import SectionMainContent from './components/SectionMainContent.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    SectionMainContent
  }
}
</script>


<style lang="scss">
@import './styles/common';

body {
  font-family: 'Encode Sans Condensed', sans-serif;
}
</style>
