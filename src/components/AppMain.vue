<template>
  <main class="main">
            <!-- struttura in comune del banner  -->
            <section id="hero-banner">
                <MyBanner />
            </section>
      -- Main Content
  </main>

</template>

<script>

import MyBanner from "./MyBanner.vue";

export default {
    name: "AppMain",
    components: {
        MyBanner,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

#hero-banner {
    background-image: url("../assets/img/slider82x-scaled.jpg");
    background-repeat: no-repeat;
    background-size:cover;
}
</style>