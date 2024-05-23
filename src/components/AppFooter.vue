<script>
export default {
    data() {
        return {
            images: [
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
        }
    },

    methods: {

    },

    mounted() {

    }
}
</script>

<template>
    <footer>
        <header class="bg-primary py-3">
            <div class="container row m-auto justify-content-evenly align-items-center">
                <div class="col-2" v-for="card in images">
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
        <main>

        </main>
        <footer>

        </footer>
    </footer>
</template>

<style></style>