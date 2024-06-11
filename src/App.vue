<script>
    import AppHeader from "./components/AppHeader.vue";
    import AppMain from "./components/AppMain.vue";
    import AppFooter from "./components/AppFooter.vue";

  export default {
    data(){

    },
    components:{
      AppHeader,
      AppMain,
      AppFooter,
    }
  }
</script>

<template>

  <AppHeader/>
  <AppMain/>
  <AppFooter/>

</template>

<style lang="scss" >
@use './style/general.scss';
@use './style/partials/mixins' as *;
@use './style/partials/variable' as *;



</style>
