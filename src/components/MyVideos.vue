<template>
    <div>
        <div class="ms-container">
            <div class="title-wrap d-flex justify-content-between align-items-center mt-5">
                <h4>Featured playlists</h4>
                <a href="">View all videos ></a>
            </div>

            <div class="container mt-3">
                <div class="row d-flex justify-content-between">
                        <div v-for="item in videosArray" :key="item" class="item col-4">                  
                            <img class="video-img" :src= "require(`../assets/img/${item.image}`)" alt="">
                        
                            <div class="wrap-text">
                                <h5 class="workout-name mb-0 mt-3 text-center">{{ item.name }}</h5>
                                <p class="workout-slogan text-center">{{ item.slogan }}</p>
                            </div>
                        </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MyVideos",
    data() {
        return {
            videosArray: [
                {
                    name: "Thighs & glute workout",
                    slogan: "Increase your mobility",
                    image: "video2-2x.jpg"
                },

                {
                    name: "Lift, firm & perk up",
                    slogan: "Feel young again",
                    image: "video7-2x.jpg"
                },

                {
                    name: "Slim & trim your waist",
                    slogan: "Shed those extra pounds",
                    image: "video9-2x.jpg"
                }
            ]
        }
    }
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

.item {
    border: 1px solid black;
    width: 30%;
     
    .video-img {
        width: 100%;
        transition: 1s;
    }

    .video-img:hover {
        border-bottom-right-radius: 25px;
    }
    .workout-name {
        font-size: 1em;
    }

    .workout-slogan {
        font-size: .8em;
        color: $dodgerblue;
    }

    .play-btn {
    background-color: white;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    border-radius: 50%;
    height: 55px;
    width: 55px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);

    i {
        color: $dodgerblue;
        font-size: .8em;
    }
}
}

</style>