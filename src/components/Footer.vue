<template>
    <div class="footer_section">
        <div class="container d-felx">
            <div class="links_box">
                <div class="links_column">
                    <div class="footer_title">DC COMICS</div>
                    <ul>
                        <li v-for="link in dcComicsLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                    <div class="footer_title">SHOP</div>
                    <ul>
                        <li v-for="link in shopllinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="links_column">
                    <div class="footer_title">DC</div>
                    <ul>
                        <li v-for="link in dcLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="links_column">
                    <div class="footer_title">SITE</div>
                    <ul>
                        <li v-for="link in sitelinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
            </div>
            <div></div>
        </div>
    </div>

</template>

<script>
export default {
    data() {
        return {
            dcComicsLinks: [
                "Characters",
                "Comics",
                "Movies",
                "Tv",
                "Games",
                "Videos",
                "News",
            ],
            dcLinks: [
                "Term Of Use",
                "Privacy Poliy",
                "Ad Choice",
                "Advertising",
                "jobs",
                "Subscriptions",
                "talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us",
            ],
            sitelinks: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa",
            ],
            shopllinks: [
                "Shop DC",
                "Shop DC Collectors"
            ]

        }
    }
}
</script>


<style scoped lang="scss">
.footer_section {
    background-color: black;
    background-image: url();
}

.links_box {
    display: flex;
    width: 500px;
}

.links_column {
    width: calc(100% / 3);

    &>ul {
        list-style: none;
        padding: 0;

        &>li>a {
            text-decoration: none;
            color: gray;
        }
    }
}

.footer_title {
    color: white;
    font-size: 1.1rem;
    font-weight: 700;
    margin: 10px 0;

}
</style>