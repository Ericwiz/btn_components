<template>
    <v-row class="mt-8">
         <v-col v-for="btn in disabledButtons" :key="btn" cols="12" md="3" class="pl-6">
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
                     {name: 'Defualt', color: 'bg-grey-lighten-2', variant: 'tonal', text: '<Button color="defualt"/>', size:"small"},
                     {name: 'Defualt', color: 'bg-blue-darken-3', variant: 'tonal', text: '<Button color="primary"/>', size:"large"},
                     {name: 'Defualt', color: 'bg-grey-darken-3', variant: 'tonal', text: '<Button color="secodry"/>', size:"x-large"},
                     {name: 'Defualt', color: 'bg-red-darken-2', variant: 'tonal', text: '<Button color="danger"/>', size:"small"},
                     {name: 'Defualt', color: 'bg-grey-darken-1', variant: 'tonal', text: '&hover, &focus', size:"large"},
                     {name: 'Defualt', color: 'bg-blue-darken-4', variant: 'tonal', size:"x-large"},
                     {name: 'Defualt', color: 'bg-grey-darken-4', variant: 'tonal', size:"small"},
                     {name: 'Defualt', color: 'bg-red-darken-4', variant: 'tonal', size:"large"},
                 ]
             }
         }
     }
 </script>
 
 <style scoped>
 
 </style>