<template>
        <!-- VIDEOCARD -->
        <div class="ms-container mt-5 mb-5">
            <div class="title-wrap d-flex justify-content-between align-items-center mt-5">
                <h4>Featured playlists</h4>
                <a href="">View all videos ></a>
            </div>

            <div class="container mt-3">
                <div class="row d-flex justify-content-between">
                    <MyVideoCard v-for="(item, idx) in videos" :key="idx" :videos="item" /> 
                </div>
            </div>
        </div>
        <!-- VIDEOCARD -->
</template>

<script>
import MyVideoCard from "./MyVideoCard.vue"
export default {
    name: "MyVideos",

    components: {
        MyVideoCard,
    },

    props: {
    videos: Array,
    },
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";



h4 {
    font-size: 1em;
}

a {
    font-size: .8em;
    color: $jumbo;
}


</style>