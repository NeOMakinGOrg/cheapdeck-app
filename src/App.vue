<template>
  <div class="cheapdeck">
    <grid />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Grid from './components/Grid.vue';

export default defineComponent({
  name: 'App',
  components: {
    Grid,
  },
});
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
}
</style>
