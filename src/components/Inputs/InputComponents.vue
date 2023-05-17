<template>
    <v-container class="w-75 h-75 m-auto">
        <h1 class="mb-10">Inputs</h1>
        <DefualtForm />
        <InputIcons />
        <InputSize />
        <InputFullwidth />
        <InputTextareaVue />
    </v-container>
</template>

<script>
import DefualtForm from './DefualtForm.vue'
import InputIcons from './InputIcons.vue'
import InputSize from './InputSize.vue';
import InputFullwidth from './InputFullwidth.vue'
import InputTextareaVue from './InputTextarea.vue'
export default {
    components: { DefualtForm, InputIcons, InputSize, InputFullwidth, InputTextareaVue }
}
</script>

<style scoped>
.border {
    border: 2px solid blue;
}
</style>