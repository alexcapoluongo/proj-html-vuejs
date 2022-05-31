<template>
  <div>
      <div class="ms-container pt-5">
          <div class="container">
              <div class="row d-flex justify-content-between">
                  <div v-for="(item,idx) in itemsArray" :key="idx" class="item p-4 pb-5 pt-5 col-4">
                      <img :src="require(`../assets/img/${item.image}`)" alt="">
                      <h3>{{ item.title }}</h3>
                      <h4>{{ item.subtitle }}</h4>
                      <p class= "mb-2">{{ item.paragraph }}</p>
                      <a href="">{{ item.link}} ></a>
                  </div>
                  <!-- <div class="item col-4">hey</div>
                  <div class="item col-4">hey</div> -->
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyPlans",
    data() {
        return {
            itemsArray: [
                {
                    image: "watch.png",
                    title: "Team training",
                    subtitle: "Find a partner",
                    paragraph: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloribus earum doloremque repellat commodi libero facere, nisi magnam veritatis temporibus totam.",
                    link: "Find a Partner"
                },

                {
                    image: "gym.png",
                    title: "Crossfit workout",
                    subtitle: "Push your limits",
                    paragraph: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloribus earum doloremque repellat commodi libero facere, nisi magnam veritatis temporibus totam.",
                    link: "Lear about Crossfit"
                },

                {
                    image: "weight.png",
                    title: "Weight loss plan",
                    subtitle: "Shed those pounds",
                    paragraph: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloribus earum doloremque repellat commodi libero facere, nisi magnam veritatis temporibus totam.",
                    link: "Schedule a workout"
                },


            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.item {
    text-align: center;
    transition: 1.5s;
    width: 30%;
    border: 2px solid transparent;

    &:hover {
        border: 2px solid $royalblue;
    }

    img {
        width: 80px;
        height: 60px;
    }

    h3 {
        color: white;
        font-size: 1em;
    }

    h4 {
        color: yellow;
        font-size: .8em;
    }

    p {
        color: $jumbo;
    }

    a {
        color: white;
        font-size: .7em;
    }
}
</style>