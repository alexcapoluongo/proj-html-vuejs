<template>
  <div>
      <div class="ms-container">
          <div class="container">
              <div class="row d-flex justify-content-between">
                  <div v-for="(item, idx) in scheduleArray" :key="idx" class="item text-center col-3">
                      <img :src="require(`../assets/img/${item.image}`)" alt="">
                      <div class="zigzag mt-2 mb-2">
                          <img src="../assets/img/zigzagblue1.png" alt="">
                      </div>
                      <p>{{ item.paragraph }}</p>
                      <a href="">{{ item.link }} ></a>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MySchedule",
    data() {
        return {
            scheduleArray: [
                {
                    image: "sponsor-1-2x.png",
                    paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse reprehenderit debitis deleniti at aperiam odit quae, blanditiis amet, ",
                    link: "Visit Yoga Studio"
                },
                {
                    image: "sponsor-2-2x.png",
                    paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse reprehenderit debitis deleniti at aperiam odit quae, blanditiis amet, ",
                    link: "Join Fitness Centre"
                },
                {
                    image: "sponsor-3-2x.png",
                    paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse reprehenderit debitis deleniti at aperiam odit quae, blanditiis amet, ",
                    link: "Learn About FC"
                },
                {
                    image: "sponsor-4-2x.png",
                    paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse reprehenderit debitis deleniti at aperiam odit quae, blanditiis amet, ",
                    link: "Visit Power Gym"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.item {
    width: 20%;

    .zigzag {
        img {
            width: 40px;
        }
    }

    img {
        width: 80%;
    }

    p {
        font-size: .8em;
        color: $jumbo;
    }

    a {
        font-size: .8em;
        color: black;
    }
}
</style>