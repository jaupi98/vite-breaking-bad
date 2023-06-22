<script>
    export default {
            props:{
                title:String
            }
        }
 </script>
<template lang="">
    <div >
        <h1 class="text-center">{{title}}</h1>
    </div>
</template>
<style lang="scss" scoped>
    div{
        height: 100vh;
        background-color: red;
        position: relative;
    }
</style>