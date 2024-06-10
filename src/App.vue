<script>
  export default {
    data(){

    },
    components:{
      AppHeader,
      AppMain,
      AppFooter
    }
  }

</script>

<template>

<AppHeader/>
<AppMain/>
<AppFooter/>

</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/mixins';
@use './style/partials/variable';
</style>
