<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#CHARACTERS",
                },
                {
                    text: "COMICS",
                    url: "#COMICS",
                },
                {
                    text: "MOVIES",
                    url: "#MOVIES",
                },
                {
                    text: "TV",
                    url: "#TV",
                },
                {
                    text: "GAMES",
                    url: "#GAMES",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#COLLECTIBLES",
                },
                {
                    text: "VIDEOS",
                    url: "#VIDEOS",
                },
                {
                    text: "FANS",
                    url: "#FANS",
                },
                {
                    text: "NEWS",
                    url: "#NEWS",
                },
                {
                    text: "SHOP",
                    url: "#SHOP",
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
    <header class="py-2 bg-white text-dark">
        <div class="container m-auto">
            <div class="row m-0 justify-content-between align-items-center">
                <figure id="logo" class="col-12 col-sm-2 col-md-1 p-2 p-sm-0 m-0 text-center">
                    <img src="/dc-logo.png" alt="" class="w-75">
                </figure>
                <nav class="col-12 col-sm-9 p-0">
                    <ul class="row m-0 p-0 justify-content-between">
                        <li v-for="link in links" class="col-12 col-sm-4 col-md-2 col-lg-1 p-0 text-center my-fs">
                            <a class="text-decoration-none hover" :href="link.url">
                                <b>{{ link.text }}</b>
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<style scoped>
a {
    color: black;
}

.hover:hover {
    color: dodgerblue;
}
</style>
