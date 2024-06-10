<script>
    export default{
        data(){
            return{

            }
        }
    }
</script>

<template>
<footer>
    <section class="container">
        <nav>
            <h2>dc comics</h2>
            <ul>
                <li>
                    <a href="#"></a>
                </li>
            </ul>
            <h2>dc</h2>
            <ul>
                <li>
                    <a href="#"></a>
                </li>
            </ul>
            <h2>sites</h2>
            <ul>
                <li>
                    <a href="#"></a>
                </li>
            </ul>
            <h2>shop</h2>
            <ul>
                <li>
                    <a href="#"></a>
                </li>
            </ul>
        </nav>
        <section> 
            <img src="../assets/img/dc-logo-bg.png" alt="dc-big-logo">
        </section>
        <section class="social">
            <button> sing-up now! </button>
        </section>
    </section>
</footer>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variable' as *;
    footer{
        background-image: url(../assets/img/footer-bg.jpg);
        .social{
            background-color: $dark-footer-bg;
            button{
                color: white;
                padding: 1rem;
                background-color: $dark-footer-bg;
                font-weight: bolder;
                text-transform: uppercase;
                border-color :$active-link-bg;
                margin: 1rem 0rem;
            }
        }
        section.container{
            width: 1200px;
            margin: 0 auto;
        }
    }

</style>