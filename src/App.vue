  <script>
  import AppHeader from './components/AppHeader.vue';
  import AppCharacters from './components/AppCharacters.vue';

    export default {
      components:{
        AppHeader,
        AppCharacters
      }
    }
  </script>

<template lang="">
  <div>
    <AppHeader title="Pokemon Apps"/>
    <AppCharacters/>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>