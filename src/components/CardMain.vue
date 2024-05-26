<script>

export default {
    name: "CardMain",
    props: ["card"],
}
</script>

<template>
    <div class="col-12 col-sm-6 col-md-4 col-lg-2 px-1">
        <figure class="m-0 h-100">
            <img :src="card.thumb" class="card-img-top img-fluid h-75" alt="">
            <h5 class="card-text my-fs py-2">{{ card.series }}</h5>
        </figure>
    </div>
</template>