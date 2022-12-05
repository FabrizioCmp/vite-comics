<template>
    <div class="bunner_section">
        <div class="container h-100">
            <div class="bunner">
                <div v-for="obj,i in listBuy" class="mycol" :key="(obj.text + i)">
                    <div>
                        <img class="img-fluid" :src="`/imgs/${obj.img}`" alt="">
                    </div>
                    <span>{{ obj.text }}</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            listBuy: [
                {
                    text: "DIGITAL COMICS",
                    img: "buy-comics-digital-comics.png",
                },
                {
                    text: "DC MERCHANDISE",
                    img: "buy-comics-merchandise.png",
                },
                {
                    text: "SUBSRIPTIONS",
                    img: "buy-comics-subscriptions.png",
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    img: "buy-comics-shop-locator.png",
                },
                {
                    text: "DC POWER VISA",
                    img: "buy-dc-power-visa.svg",
                },
            ]

        }
    }
}
</script>


<style scoped lang="scss">
.bunner_section {
    background-color: #0282F9;
}

.bunner {
    height: 150px;
    display: flex;
    
    width: 100%;
}

.mycol {
    width: calc(100% / 5);
    display: flex;
    align-items: center;
    column-gap: 1rem;

    span{
        font-size: .8rem;
        color: white;
    }

    div{
        height:  40px;
        
        img{
            
            height: 100%;
        }
    }
}
</style>