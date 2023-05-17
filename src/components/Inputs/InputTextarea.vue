<template>
    <v-row>
        <v-col cols="12" v-for="iconInput in defualtInputs" :key="iconInput">
            <p class="pb-4 text-caption">{{ iconInput.text }}</p>
            <label class="text-capitalize d-block" :class="iconInput.labelStyle">{{ iconInput.label }}</label>
             <textarea 
             type="text" class="rounded-lg px-2 py-3"  
             :placeholder="iconInput.placeholder" :class="iconInput.style" 
             > </textarea>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        data() {
            return {
                defualtInputs: [
                    {label: 'label', placeholder: 'placeholder', text: '<input multiline rows="4" />', style: 'general border-grey-1', labelStyle: 'text-grey-darken-1'},
                ]
            }
        }
    }
</script>

<style scoped>
.general {
    outline: none;
}
.border-grey-1 {
    border: 2px solid #E0E0E0;
}

</style>