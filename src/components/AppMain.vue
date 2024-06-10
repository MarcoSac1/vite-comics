<script>
    export default{
        data(){
            return{

            }
        }
    }
</script>

<template>
<main>
    <section class="text">
        <p>--> Contents goes here <-- </p>
    </section>
</main>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variable' as *;
    
    main {
        background-color: $dark-main-bg;
        color: white;
        padding: 4rem;
        font-size: 1.5rem;
            
        .text{
            width: 1200px;
            margin: 0 auto;
        }
    }


</style>