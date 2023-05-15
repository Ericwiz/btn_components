<template>
    <row>
        <v-col cols="1" md="6">
            <v-btn></v-btn>
        </v-col>
    </row>
</template>

<script>
    export default {
        data() {
            return {
                disabledButtons: [
                    {name: 'Disabled', color: '', variant: ''}
                ]
            }
        }
    }
</script>

<style scoped>

</style>