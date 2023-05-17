<template>
    <v-container class="w-75 h-75 m-auto">
        <h1 class="mb-10">Inputs</h1>
        <DefualtForm />
    </v-container>
</template>

<script>
import DefualtForm from './DefualtForm.vue'
export default {
    components: {DefualtForm}
}
</script>

<style scoped>
.border {
    border: 2px solid blue;
}
</style>