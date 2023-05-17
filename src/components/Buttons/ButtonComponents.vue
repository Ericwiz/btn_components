<template>
  <v-container class="w-75 h-75 m-auto">
    <h1 class="mb-10">Buttons</h1>
    <DefualtButtonVue />
    <DisabledButton />
    <IconButton />
    <SizedButton />
    <DangerButtons />
    <div class="text-left text-caption mt-16">
  </div>
  </v-container>
</template>

<script>
import DangerButtons from './DangerButtons.vue';
import DefualtButtonVue from './DefualtButton.vue';
import DisabledButton from './DisabledButton.vue';
import IconButton from './IconButton.vue';
import SizedButton from './SizedButton.vue';
  export default {
    components: { DefualtButtonVue, DisabledButton, IconButton, SizedButton, DangerButtons }
  }
</script>

<style scoped>

</style>