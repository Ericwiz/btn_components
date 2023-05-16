<template>
    <v-row class="mt-8">
         <v-col v-for="btn in disabledButtons" :key="btn" cols="12" md="6">
             <p class="pb-4 text-caption">{{ btn.text }}</p>
             <v-btn :variant="btn.variant" class="rounded-lg" :class="btn.color" :prepend-icon="btn.prependIcon" :append-icon="btn.appendIcon" >{{ btn.name }}</v-btn>
         </v-col>
     </v-row>
 </template>
 
 <script>
     export default {
         data() {
             return {
                 disabledButtons: [
                     {name: 'Defualt', color: 'bg-blue-darken-2', 
                     variant: 'tonal', text: '<Button startIcon="mdi-cellphone-arrow-down"/>', 
                     prependIcon: 'mdi-cellphone-arrow-down'},
                     {name: 'Disabled', color: 'bg-blue-darken-2', 
                     variant: 'text', text: '<Button endIcon="mdi-cellphone-arrow-down"/>', 
                     appendIcon: 'mdi-cellphone-arrow-down'}
                 ]
             }
         }
     }
 </script>
 
 <style scoped>
 
 </style>