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
      <MainBanner/>
      <ProductsSection/>
      <SectionShop/>
    </main>

    <MyFooterTop/>
    <MyFooterBottom/>
  </div>
</template>


<script>
import MyHeader from './components/MyHeader.vue';
import ProductsSection from './components/ProductsSection.vue';
import SectionShop from './components/SectionShop.vue';
import MyFooterTop from './components/MyFooterTop.vue';
import MyFooterBottom from './components/MyFooterBottom.vue';
import MainBanner from './components/MainBanner.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    ProductsSection,
    SectionShop,
    MyFooterTop,
    MyFooterBottom,
    MainBanner
  }
}
</script>


<style lang="scss">
@import './styles/common';
@import './styles/variables';

body {
  font-family: 'Encode Sans Condensed', sans-serif;
  color: $almost_black;
}
</style>
