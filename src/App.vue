<script>
import {store} from './store';

import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  
  data() {
    return {
      store
    }
  },

  components:{
    HeaderApp,
    MainApp,
    FooterApp,
  },
}

</script>

<template>

  <HeaderApp />

  <MainApp />

  <FooterApp />

</template>

<style lang="scss">
  @use "./styles/main.scss";
</style>
