<template>
  <div class="banner">

        <div class="ms-container pt-5">
            <h3 class="mt-3">Certified fitness professional</h3>
            <h1>Take control of your health</h1>
                <div class="zigzag">
                    <img src="../assets/img/zigzagyellow1.png" alt="">
                </div>       	
                <MyHeroBanner v-if="hasButtons"/>         
                <MyMailingList v-if="hasInput"/>
        </div>
    </div>
</template>

<script>
import MyHeroBanner from "./MyHeroBanner.vue"
import MyMailingList from "./MyMailingList.vue"

export default {
    name: "MyBanner",
    props: {
        hasButtons: Boolean,
        hasInput: Boolean,
    },
    components: {
        MyHeroBanner,
        MyMailingList,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.banner {
    height: 500px;

    h3 {
        color: $monza;
        font-size: 1em;
    }

    h1 {
        color: white;
    }  

}

.ms-container {
    background: linear-gradient(90deg, rgba(0,0,0,1) 40%, rgba(0,0,0,0) 97%);
}
</style>