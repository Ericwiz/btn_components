<template>
  <v-container class="w-75 h-75 m-auto">
    <h1 class="mb-10">Buttons</h1>
    <DefualtButtonVue />
    <DisabledButton />
  </v-container>
</template>

<script>
import DefualtButtonVue from './DefualtButton.vue';
import DisabledButton from './DisabledButton.vue';
  export default {
    components: {DefualtButtonVue, DisabledButton}
  }
</script>

<style scoped>

</style>