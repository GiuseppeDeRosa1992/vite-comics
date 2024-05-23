<script>
export default {
    data() {
        return {
            cards: [
                {
                    text: "DIGITAL COMICS",
                    search: "./card-dc.png",
                },
                {
                    text: "DC MERCHANDISE",
                    search: "./merchandise.png",
                },
                {
                    text: "SUBSCRIPTION",
                    search: "./subscriptions.png",
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    search: "./shop-locator.png",
                },
                {
                    text: "DC POWER VISA",
                    search: "./dc-power-visa.svg",
                },
            ],

            images: [
                {
                    src: "./footer-facebook.png",
                },
                {
                    src: "./footer-twitter.png",
                },
                {
                    src: "./footer-youtube.png",
                },
                {
                    src: "./footer-pinterest.png",
                },
                {
                    src: "./footer-periscope.png",
                },
            ],
        }
    },

    methods: {

    },

    mounted() {

    }
}
</script>

<template>
    <!-- Suddivido Footer in 3 sezioni header main e footer -->
    <footer>
        <!-- Aggiuto header del footer con le img e il background azzurro -->
        <header class="bg-primary py-3">
            <div class="container row m-auto justify-content-evenly align-items-center">
                <div class="col-2" v-for="card in cards">
                    <div class="row m-0 align-items-center py-3">
                        <figure class="col-4 m-0">
                            <img :src="card.search" alt="" class="img-fluid">
                        </figure>
                        <h5 class="col-8 m-0 my-fs">
                            {{ card.text }}
                        </h5>
                    </div>
                </div>
            </div>
        </header>
        <!-- aggiungo il main del footer con background image e link vari -->
        <main class="py-3">

        </main>
        <!--  aggiungo footer del footer con bottone a sinistra e a destra le varie img social -->
        <footer class="py-4 bg-footer">
            <div class="container row m-auto justify-content-between align-items-center">
                <div class="col-2">
                    <button type="button" class="btn btn-outline-info text-white">SIGN-UP NOW!</button>
                </div>
                <div class="col-8 text-end">
                    <span class="text-primary p-1">FOLLOW US</span>
                    <img :src="img.src" alt="" v-for="img in images" class="px-2">
                </div>
            </div>
        </footer>
    </footer>
</template>

<style>
.bg-footer {
    background-color: #303030;
}
</style>