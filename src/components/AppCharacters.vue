<script>
import axios from 'axios';
import AppCharacter

    export default {
            data(){
                return{
                    pokemonList:[]
                }
            },
            mounted() {
                axios.get('https://41tyokboji.execute-api.eu-central-1.amazonaws.com/dev/api/v1/pokemons?eq[type1]=Electric&sort[number]=desc').then((response) =>{
                    this.pokemonList = response.data.docs;
                }
                )
            },
        }
 </script>
<template lang="">
    <div class="interno">
        <div class="container">
            <div class="row">
                <div v-for="(pokemon,index) in pokemonList " :key="index" class="col-6 col-md-2">
                
                </div>
            </div>
        </div>

       
    </div>
</template>

<style lang="scss" scoped>

.interno{
    position: absolute;
    top: 100px;
    left: 100px;
    right: 100px;
    bottom: 100px;
    background-color: blue;
}


</style>