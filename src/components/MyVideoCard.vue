<template>
        <div class="item col-4"> 
            <div class="container-img">          
                <img class="video-img" :src= "require(`../assets/img/${videos.image}`)" alt="">
                <div class="play-btn">
                    <i class="fas fa-play"></i>
                </div>
            </div>
            <div class="wrap-text">
                <h5 class="workout-name mb-0 mt-3 text-center">{{ videos.name }}</h5>
                <p class="workout-slogan text-center">{{ videos.slogan }}</p>
            </div>
        </div>                  
</template>

<script>
export default {
    name: "MyVideoCard",
    props: {
        videos:Object,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.container-img {
    position:relative;
    display:inline-block;

    i {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
    }
}

.item {
    width: 30%;
     
    .video-img {
        width: 100%;
        transition: 1s;
        position: relative;

        &:after {
        content: '';
        position: absolute;
        width: 100%; height:100%;
        top:0; left:0;
        background:rgba(0,0,0,0.6);
        opacity: .5;  
        }

    }

    .video-img:hover {
        border-bottom-right-radius: 25px;
        filter:brightness(70%)
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