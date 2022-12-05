<template>
    <div class="container">
        <div class="navbar">
            <div class="icon_dc">
                <img class="img-fluid" src="/imgs/dc-logo.png" alt="">
            </div>

            <div class="menu">
                <ul>
                    <li v-for="menuitem,i in listMenu" :key="menuitem + i"><a href="#">{{ menuitem.toUpperCase() }}</a></li>
                </ul>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    data() {
        return {
            listMenu: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop",
            ]
        }
    }
}
</script>


<style scoped lang="scss">
.navbar {
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .icon_dc {
        height: 100%;

        img {
            height: 100%;
        }
    }
}

.menu {
    ul {
        display: flex;
        list-style: none;
        column-gap: 1.5rem;
        align-items: center;
        padding: 0;
        margin: 0;
        font-weight: 600;
        font-size: .8rem;
        
        li > a{
            text-decoration: none;
            color: black;
        }
    }
}
</style>