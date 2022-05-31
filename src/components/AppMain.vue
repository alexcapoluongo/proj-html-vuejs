<template>
  <main class="main">
            <!-- struttura in comune del banner  -->
            <section id="hero-banner" class="mt-5">
                <MyBanner /> 
            </section>

            <section class="services" id="services">
                <MyServices />
            </section>

            <section class="about" id="about">
                <MyAbout />
            </section>

            <section class="videos" id="videos">
                <MyVideos />
            </section>

            <section class="mailing-list" id="mailing-list">
                <MyBanner />
            </section>

            <section class="plans" id="plans">
                <MyPlans />
            </section>

            <section class="blog" id="blog">
                <MyVideos />
            </section>
      -- Main Content
  </main>

</template>

<script>

import MyBanner from "./MyBanner.vue";
import MyServices from "./MyServices.vue";
import MyAbout from "./MyAbout.vue";
import MyVideos from "./MyVideos.vue";
import MyPlans from "./MyPlans.vue";



export default {
    name: "AppMain",
    components: {
        MyBanner,
        MyServices,
        MyAbout,
        MyVideos,
        MyPlans,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

#hero-banner {
    background-image:url(../assets/img/slider82x-scaled.jpg);
    background-size: cover;
}

#services {
    background: rgb(4,19,255);
    background: linear-gradient(150deg, rgba(4,19,255,1) 10%, rgba(255,0,0,1) 100%);
}

#mailing-list {
    background-image: url(../assets/img/banner1-2x.jpg);
    background-size: cover;
}

#plans {
    height: 500px;
    background: black;
}

</style>