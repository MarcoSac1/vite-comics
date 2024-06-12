<script>
export default{
    data(){
        return{
            
        }
    }
}
</script>
<template>
    <section class="jumbo">
        <img src="../assets/img/jumbotron.jpg" alt="jumbo_img">
        <button> current series</button>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;

    section.jumbo{
        padding: 4rem;
        
    }
    button{
        border: none;
        padding: .5rem 2.5rem;
        background-color:$active-link-bg ;
        color: white;
        text-transform: uppercase;
        font-weight: bolder;
    }   
</style>