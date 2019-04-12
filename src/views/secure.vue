<template>
    <div id="secure">
        <div class="buttons">
            <b-button  v-on:click="table()" type="is-primary">Cargar</b-button>

          
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Secure',
        data() {
            return {};
        },
        methods:{
            table(){
                this.$router.replace({ name: "table" });
            }


        }

    }
</script>

<style scoped>
    #secure {
        background-color: #FFFFFF;
        border: 1px solid #CCCCCC;
        padding: 20px;
        margin-top: 10px;
    }
</style>