<script>
    import ListProduct from './ListProduct.vue';
    import JumbotronSection from './JumbotronSection.vue';
    export default{
        data(){
            
        },
        components:{
        ListProduct,
        JumbotronSection
        }
    }
    
</script>

<template>
    <main>
        <section>
            <JumbotronSection/>
        </section>
        <section class="text">
            <ListProduct/>
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
            color: white;
        }
    }


</style>