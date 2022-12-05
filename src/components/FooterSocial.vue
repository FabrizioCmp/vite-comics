<template>
    <div class="social_section">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="btn_signup">
                <a href="">SIGN-UP NOW!</a>
            </div>
            <div class="social_links">
                    <h5>FOLLOW US</h5>
                    <ul>
                        <li v-for="img in imgsSocialList ">
                            <a href="#">
                                <img :src="`/imgs/${img}`" alt="">
                            </a>
                        </li>
                    </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            imgsSocialList: [
                "footer-facebook.png",
                "footer-twitter.png",
                "footer-youtube.png",
                "footer-pinterest.png",
                "footer-periscope.png",
            ]
        }
    }
}
</script>


<style scoped lang="scss">
.social_section {
    background-color: #303030;
    padding: 3rem;
}

.btn_signup {
    background-color: transparent;
    padding: .3rem .5rem;
    border: 2px solid #0282F9;

    a {
        text-decoration: none;
        color: white;
        font-size: .8rem;
    }
}

.social_links {
    display: flex;
    align-items: center;

    h5 {
        color: #0282F9;
        margin: 0;
    }

    ul{
        display: flex;
        align-items: center;
        column-gap: 20px;
        margin: 0;
        margin-left: 20px;  
        padding: 0;
        list-style: none;
        text-decoration: none;
    }
}
</style>