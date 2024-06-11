<script>
    export default{
        data(){
            return{
                footerLinks: [
                    {
                        id: 1,
                        title:'characters',
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'comics',
                        url:'#',
                    },
                    {
                        id: 3,
                        title:'movies',
                        url:'#',
                    },
                    {
                        id: 4,
                        title:'tv',
                        url:'#',
                    },
                    {
                        id: 5,
                        title:'games',
                        url:'#',
                    },
                    {
                        id: 6,
                        title:'collectibles',
                        url:'#',
                    },
                    {
                        id: 7,
                        title:'videos',
                        url:'#',
                    },
                    {
                        id: 8,
                        title:'fans',
                        url:'#',
                    },
                    {
                        id: 9,
                        title:'news',
                        url:'#',
                    },
                    {
                        id: 10,
                        title:'shop',
                        url:'#',
                    },
                ],
                footerTermOfUse: [
                    {
                        id: 1,
                        title:'Terms Of Use',
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'Privaci policy (New)',
                        url:'#',
                    },
                    {
                        id: 3,
                        title:'Ad choices',
                        url:'#',
                    },
                    {
                        id: 4,
                        title:'Advertising',
                        url:'#',
                    },
                    {
                        id: 5,
                        title:'Jobs',
                        url:'#',
                    },
                    {
                        id: 6,
                        title:'Subscriptions',
                        url:'#',
                    },
                    {
                        id: 7,
                        title:'Talent Workshops',
                        url:'#',
                    },
                    {
                        id: 8,
                        title:'CPSC Certificates',
                        url:'#',
                    },
                    {
                        id: 9,
                        title:'Ratings',
                        url:'#',
                    },
                    {
                        id: 10,
                        title:'Show Help',
                        url:'#',
                    },
                    {
                        id: 11,
                        title:'Contact Us',
                        url:'#',
                    },
                ],
                footerShop: [
                    {
                        id: 1,
                        title:'Shop DC',
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'Shop DC Collectibles',
                        url:'#',
                    },
                ],
                footerSites: [
                    {
                        id: 1,
                        title:'DC',
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'MAD Magazine',
                        url:'#',
                    },
                    {
                        id: 3,
                        title:'DC Kids',
                        url:'#',
                    },
                    {
                        id: 4,
                        title:'DC Universe',
                        url:'#',
                    },
                    {
                        id: 5,
                        title:'DC Power Visa',
                        url:'#',
                    },
                ],
                footerSocialIcon: [
                    {
                        id: 1,
                        // title:url(..),
                        url:'#',
                    },
                    {
                        id: 2,
                        title:'MAD Magazine',
                        url:'#',
                    },
                    {
                        id: 3,
                        title:'DC Kids',
                        url:'#',
                    },
                    {
                        id: 4,
                        title:'DC Universe',
                        url:'#',
                    },
                    {
                        id: 5,
                        title:'DC Power Visa',
                        url:'#',
                    },
                ],
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
                <li v-for="link in footerLinks"  :key="link.id">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
            <h2>shop</h2>
            <ul>
                <li v-for="link in footerShop"  :key="link.id">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>>
            </ul>
            <h2>dc</h2>
            <ul>
                <li v-for="link in footerTermOfUse"  :key="link.id">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
            <h2>sites</h2>
            <ul>
                <li v-for="link in footerSites"  :key="link.id">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
        </nav>
        <section class="img"> 
            <img src="../assets/img/dc-logo-bg.png" alt="dc-big-logo">
        </section>
        </section>
        <section class="social">
            <section class="sing">
                <button> sing-up now! </button>
            </section>
            <section class="follow">
                <h2>follow us</h2>
            <ul>
                <li v-for="link in footerSocialIcon"  :key="link.id">
                    <a :href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
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
            .sing{
                width: 1200px;
                margin: 0 auto;
            }
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
        .container{
            display: flex;
            width: 1200px;
            height: 400px;
            margin: 0 auto;
            padding: 1rem;
        }
        nav{
            width: 600px;
            display: flex;
            align-items: flex-start;
            flex-direction: column;
            flex-wrap: wrap;
        ul{
            flex-direction: column;
            flex-wrap: wrap;
            list-style-type: none;
            // margin-bottom: .2rem;
                li{
                    font-size: .6rem;
                    padding: .3rem .0rem;
                    font-weight: 600;
                }
            }
        }
        section.img{
            width: 100%;
            object-fit: cover;
            display: flex;
            justify-content: flex-end;
        }
        a{
            color:#858b8f;
            text-decoration: none;
        }
        h2{
            color: white;
            text-transform: uppercase;
            margin-bottom: 1rem;
        }
        section.follow{
            h2{
                color:$active-link-bg;
            }
            display: flex;
            justify-content: center;
            align-items: center;
            ul{
                display: flex;
                list-style-type: none;
            }
        }
    }

</style>