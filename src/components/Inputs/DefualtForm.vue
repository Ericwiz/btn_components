<template>
    <v-row>
        <v-col cols="12" md="6" lg="4" v-for="defualtInput in defualtInputs" :key="defualtInput">
            <p class="pb-4 text-caption">{{ defualtInput.text }}</p>
            <label class="text-capitalize d-block" :class="defualtInput.labelStyle">{{ defualtInput.label }}</label>
             <input type="text" class="rounded-lg px-2 py-3" :placeholder="defualtInput.placeholder"  :disabled="defualtInput.disabled" :class="defualtInput.style">
        </v-col>
    </v-row>
</template>

<script>
    export default {
        data() {
            return {
                defualtInputs: [
                    {label: 'label', placeholder: 'placeholder', text: '<input />', style: 'general w-75 border-grey-1', labelStyle: 'text-grey-darken-1'},

                    {label: 'label', placeholder: 'placeholder', text: '&:hover', style: 'general w-75 border-grey-2', labelStyle: 'text-grey-darken-1'},

                    {label: 'label', placeholder: 'placeholder', text: '&:focus', style: 'general w-75 border-light-blue', labelStyle: 'text-blue-darken-1'},

                    {label: 'label', placeholder: 'placeholder', text: '<input error />', style: 'general w-75 border-red-1', labelStyle: 'text-red'},

                    {label: 'label', placeholder: 'placeholder', text: '&:hover', style: 'general w-75 border-grey-2', labelStyle: 'text-grey-darken-1'},

                    {label: 'label', placeholder: 'placeholder', text: '&:focus', style: 'general w-75 border-red-2', labelStyle: 'text-red'},

                    {label: 'label', placeholder: 'placeholder', text: '<input disabled />', style: 'general w-75 bg-grey-lighten-3', labelStyle: 'text-grey-darken-1', disabled: true},
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
</style>