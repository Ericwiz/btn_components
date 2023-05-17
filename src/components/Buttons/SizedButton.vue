<template>
    <v-row class="mt-8">
         <v-col v-for="btn in disabledButtons" :key="btn" cols="12" md="4">
             <p class="pb-4 text-caption">{{ btn.text }}</p>
             <v-btn :variant="btn.variant" class="rounded-lg" :class="btn.color" :size="btn.size">{{ btn.name }}</v-btn>
         </v-col>
     </v-row>
 </template>
 
 <script>
     export default {
         data() {
             return {
                 disabledButtons: [
                     {name: 'Defualt', color: 'bg-blue-darken-2', variant: 'tonal', text: '<Button size="sm"/>', size:"small"},
                     {name: 'Defualt', color: 'bg-blue-darken-2', variant: 'tonal', text: '<Button size="md"/>', size:"large"},
                     {name: 'Defualt', color: 'bg-blue-darken-2', variant: 'tonal', text: '<Button size="lg"/>', size:"x-large"},
                 ]
             }
         }
     }
 </script>
 
 <style scoped>
 
 </style>