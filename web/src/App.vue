<template>
  <div>
    <div>Bot name:{{ bot_name }}</div>

    <div>Bot rating:{{ bot_rating }}</div>
  </div>
  <router-view />
</template>

<script>
import { ref } from 'vue';

export default {
  name: 'App',
  setup: () => {
    let bot_name = ref('');
    let bot_rating = ref('');
    return {
      bot_name,
      bot_rating,
    };
  },
}
</script>

<style></style>
