<script>
    export default{
        data(){
            return{
                headerLinks: [
                    {
                        id: 1,
                        title:'characters',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'comics',
                        active:true,
                        url:'#',
                    },
                    {
                        id: 3,
                        title:'movies',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 4,
                        title:'tv',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 5,
                        title:'games',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 6,
                        title:'collectibles',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 7,
                        title:'videos',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 8,
                        title:'fans',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 9,
                        title:'news',
                        active:false,
                        url:'#',
                    },
                    {
                        id: 10,
                        title:'shop',
                        active:false,
                        url:'#',
                    },
                ]
            }
        }
    }
</script>

<template>
<header>
    
    <section  class="logo">
        <img src="../assets/img/dc-logo.png" alt="DC-main-logo" >
    </section>
    <section class="navbar">
        <nav>
            <ul>
                <li v-for="link in headerLinks"  :key="link.id" class="(link.active) ? 'active' ''">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
        </nav>
    </section>
</header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable.scss' as *;

    header{
        display: flex;
        flex-direction: row;
        align-items: center;
        padding: 1rem;
        margin-bottom: 4rem;
    }

    img{
        width: 4rem;
    }

    .logo{
        width: 50%; 
        display: flex;
    }

    nav {
        width: 100%;
        ul{
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            list-style-type: none;
                li{
                    font-size: .8rem;
                    padding: .5rem;
                    font-weight: 600;
                    text-transform: uppercase;
                    &.active{
                        background-color: $active-link-bg;
                    }
                }
        }

        a{
            color: black;
            text-decoration: none;
        }
    }
</style>