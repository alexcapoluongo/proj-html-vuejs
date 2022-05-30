<template>
  <div>
      <div class="ms-container">
        <div class="container">
            <div class="row">
                <div v-for="item in servicesArray" :key="item" class="col">         
                    <div class="item">
                        <div class="text-wrap mx-3">
                            <span>____</span>
                            <h3 class="mb-0">{{ item.service }}</h3>
                            <p>{{ item.slogan }}</p>
                        </div>
                    </div> 
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyServicesGrid",

    data() {
        return {
            servicesArray: [
                {
                    service: "Crossfit workout",
                    slogan: "Push your limits"   
                },
                {
                    service: "New gym apparel",
                    slogan: "Look good, feel good"   
                },
                {
                    service: "Team training",
                    slogan: "Find a partner"   
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.item {
    height: 250px;
    border: 1px solid black;
    width: 250px;
    margin: auto;
    display: flex;
    justify-content: flex-end;
    flex-direction: column;
    background-image:url("../assets/img/service6-2x.jpg");
    background-size:cover;

    .text-wrap {
        border: 1px solid purple;
        height: 100px;
        width: 100%;

        span {
            color:red;
            font-size:bolder;
        }

        h3 {
            color:white;
            font-size: 1.5em;
        }

        p {
            color: yellow;
        }
    }
}

</style>