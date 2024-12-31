<template>
  <NavBar />
  <router-view />
</template>

<script>
import NavBar from './components/NavBar.vue';
import "bootstrap/dist/css/bootstrap.min.css";
import "bootstrap/dist/js/bootstrap.min.js";

'import $ from jquery;'
import { ref } from 'vue';

export default {
  components: {
    NavBar,
  },
  setup() {
    const bot_name = ref('Bot name');
    const bot_rating = ref('Bot rating');

    return {
      bot_name,
      bot_rating,
    };
  },

}
</script>


<style>
body {
  background-image: url('@/assets/images/background.webp');
  background-size: cover;
}
</style>
