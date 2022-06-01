<template>
        <div class="item col-4"> 
            <div class="container-img">          
                <img class="video-img" :src= "require(`../assets/img/${articles.image}`)" alt="">
            </div>
            <div class="wrap-text">
                <h5 class="workout-name mb-0 mt-3 text-center">{{ articles.name }}</h5>
                <p class="workout-slogan text-center">{{ articles.author }}</p>
            </div>
        </div>                  
</template>

<script>
export default {
    name: "MyArticleCard",
    props: {
        articles:Object,
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
        color: $jumbo;
    }

}
</style>

