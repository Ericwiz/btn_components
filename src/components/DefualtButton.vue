<template>
    <v-row>
        <v-col v-for="btn in defualtButtons" :key="btn" cols="12" md="6">
            <p class="pb-4 text-body-2">{{ btn.text }}</p>
            <v-btn :variant="btn.variant" class="rounded-lg" :class="btn.color">{{ btn.name }}</v-btn>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        data() {
            return {
                defualtButtons: [
                    {name: 'Defualt', color: '', variant: 'tonal', text: '<Button />'},
                    {name: 'Defualt', color: 'bg-grey-lighten-1', variant: 'flat', text: '&hover, &focus'},
                    {name: 'Defualt', color: 'text-blue', variant: 'outlined', text: '<Button variant="outline"/>'},
                    {name: 'Defualt', color: 'text-blue bg-blue-lighten-5', variant: 'outlined', text: '&hover, &focus'},
                    {name: 'Defualt', color: 'text-blue', variant: '', text: '<Button variant="text"/>'},
                    {name: 'Defualt', color: 'text-blue bg-blue-lighten-5', variant: '', text: '&hover, &focus'},
                    {name: 'Defualt', color: 'bg-blue-darken-2', variant: '', text: '<Button variant="disabledShadow"/>', disabled: 'true'},
                ]
            }
        }
    }
</script>

<style scoped>

</style>