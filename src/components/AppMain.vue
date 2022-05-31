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

            <section class="store" id="store">
                <MyStore />
            </section>

            <section class="schedule" id="schedule">
                <MySchedule />
            </section>

            <section class="daily-workout" id="daily-workout">
                <MyDailyWorkout />
            </section>
  </main>

</template>

<script>

import MyBanner from "./MyBanner.vue";
import MyServices from "./MyServices.vue";
import MyAbout from "./MyAbout.vue";
import MyVideos from "./MyVideos.vue";
import MyPlans from "./MyPlans.vue";
import MyStore from "./MyStore.vue";
import MySchedule from "./MySchedule.vue";
import MyDailyWorkout from "./MyDailyWorkout.vue";


export default {
    name: "AppMain",
    components: {
        MyBanner,
        MyServices,
        MyAbout,
        MyVideos,
        MyPlans,
        MyStore,
        MySchedule,
        MyDailyWorkout
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

#store {
    height: 500px;
    color: white;
    background-image:url(../assets/img/banner2-2x.jpg);
    background-size: cover;
}

#schedule {
    padding-top:100px;
    padding-bottom:100px;
}

#daily-workout {
    height: 500px;
    color: white;
    background-image:url(../assets/img/banner14-2x.jpg);
    background-size: cover;
   

}

</style>