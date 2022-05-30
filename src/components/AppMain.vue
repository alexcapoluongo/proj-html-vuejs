<template>
  <main class="main">
            <!-- struttura in comune del banner  -->
            <section id="hero-banner" class="mt-5">
                <MyBanner />
            </section>

            <section class="services">
                <MyServicesGrid />
            </section>
      -- Main Content
  </main>

</template>

<script>

import MyBanner from "./MyBanner.vue";
import MyServicesGrid from "./MyServicesGrid.vue";

export default {
    name: "AppMain",
    components: {
        MyBanner,
        MyServicesGrid,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

#hero-banner {
    background-image:url(../assets/img/slider82x-scaled.jpg);
    background-size: cover;

}

.services {
    height: 400px;
}
</style>