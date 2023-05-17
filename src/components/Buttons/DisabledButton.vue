<template>
   <v-row>
        <v-col v-for="btn in disabledButtons" :key="btn" cols="12" md="6">
            <p class="pb-4 text-caption">{{ btn.text }}</p>
            <v-btn :variant="btn.variant" class="rounded-lg" :class="btn.color">{{ btn.name }}</v-btn>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        data() {
            return {
                disabledButtons: [
                    {name: 'Disabled', color: 'bg-grey-lighten-1', variant: 'tonal', text: '<Button disabled/>'},
                    {name: 'Disabled', color: '', variant: 'text', text: '<Button variant="text" disabled/>'}
                ]
            }
        }
    }
</script>

<style scoped>

</style>