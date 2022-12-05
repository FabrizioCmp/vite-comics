<template>
    <div class="bkg_jumbo"></div>
    <div class="content_section">
        
        <div class="container">
            <div class="content_box">
                <div class="content_title">CURRENT SERIES</div>
                <div class="cards_box">
                    <div class="row flex-wrap">
                        <div v-for="item in contentList" class="col-2" :key="(item.series + i)">
                            <div class="my_card">
                                <img :src="item.thumb" alt="">
                                <div>{{item.series}}</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>


<script>
import myjson from "../assets/JSON/dc-comics.json";

export default {
    data() {
        return {
            contentList: myjson
        }
    },
    methods:{
        
    }
}
</script>


<style scoped lang="scss">
.bkg_jumbo {
    height: 400px;
    background-image: url("/imgs/jumbotron.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}

.content_section {
    min-height: 100px;
    background-color: #1C1C1C;
}

.content_box {
    color: white;
    display: flex;
    align-items: center;
    position: relative;
        .content_title{
            position: absolute;
            top: -20px;
            background-color:  #0282F9;
            padding: .5rem 2rem;
            font-weight: 700;
        }
}
.cards_box{
    width: 100%;
    margin-top: 3rem;
}

.my_card{
    img{
        object-fit: cover;
        height: 200px;
    }
}
</style>