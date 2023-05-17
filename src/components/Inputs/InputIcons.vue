<template>
    <v-row>
        <v-col cols="12" md="6" v-for="iconInput in defualtInputs" :key="iconInput">
            <p class="pb-4 text-caption">{{ iconInput.text }}</p>
            <label class="text-capitalize d-block" :class="iconInput.labelStyle">{{ iconInput.label }}</label>
             <input 
             :value="iconInput.value"
             type="text" class="rounded-lg px-2 py-3"  
             :disabled="iconInput.disabled" 
             :placeholder="iconInput.placeholder" :class="iconInput.style" 
             v-show="iconInput.show">
             <v-text-field 
             type="text" 
             v-show="iconInput.apendIcon" 
             :append-inner-icon="iconInput.aIcon"
             :prepend-inner-icon="iconInput.pIcon"
             :placeholder="iconInput.placeholder"/>
             <p class="pt-2 text-caption" :class="iconInput.labelStyle">{{ iconInput.helperText }}</p>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        data() {
            return {
                defualtInputs: [
                    {label: 'label', placeholder: 'placeholder', text: '<input helperText="some interesting text" text />', style: 'general w-75 border-grey-1', labelStyle: 'text-grey-darken-1', helperText:'some interesting text', show: true},

                    {label: 'label', placeholder: 'placeholder', text: '<input helperText="some interesting text" error />', style: 'general w-75 border-red-1', labelStyle: 'text-red', helperText:'some interesting text', show: true},

                    {label: 'label', placeholder: 'placeholder', text: '<input startIcon />', style: 'general w-75 border-light-blue', labelStyle: 'text-grey-darken-1', prependIcon: 'true', apendIcon: true, show: false, pIcon: 'mdi-music-circle'},

                    {label: 'label', placeholder: 'placeholder', text: '<input endIcon />', style: 'general w-75 border-red-1', labelStyle: 'text-grey-darken-1', apendIcon: true, show: false, aIcon: 'mdi-music-box'},

                    {label: 'label', value: 'Text', text: '<input value="Text">', style: 'general w-75 border-grey-2', labelStyle: 'text-grey-darken-1', show: true,},
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
.border-grey-2 {
    border: 2px solid #BDBDBD;
}

.border-light-blue {
    border: 2px solid #039BE5;
}

.border-red-1 {
    border: 2px solid #EF5350;
}
.border-red-2 {
    border: 2px solid #D32F2F;
}

.background{
    background-color: red;
}
.input-position {
    position: relative;
    background-color: #039BE5;
}
.icon-position-1 {
    position: absolute;
    right: 18rem;
    padding-top: 20px;
}
</style>