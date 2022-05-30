<template>
  <div>
      <div class="ms-container">
        <div class="container">
            <!-- grid -->
            <div class="row">
                <div v-for="item in servicesArray" :key="item" class="col">         
                    <div class="item" :style="{'background-image': 'url(' + require(`../assets/img/${item.image}`) + ')'}">
                        <div class="text-wrap mx-3">
                            <span class="text-center">____</span>
                            <h3 class="mb-0">{{ item.service }}</h3>
                            <p>{{ item.slogan }}</p>
                        </div>
                    </div> 
                </div>
            </div>

            <!-- user-overview -->
            <div class="overview m-auto mt-5">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora veritatis nam dignissimos. Natus unde vel culpa quae perferendis fugit saepe recusandae, qui repudiandae necessitatibus quia deleniti perspiciatis officia, quod quidem. <br> <span>_____</span></p>
                
                <div class="user">

                    <img src="../assets/img/video2-2x.jpg" alt="">

                    <ul class="px-1 pb-5">
                        <li><span id="username">Brad Johnson</span></li>
                        <li><span id="user-city">Las Vegas</span></li>
                    </ul>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyServices",

    data() {
        return {
            servicesArray: [
                {
                    image: "service6-2x.jpg",
                    service: "Crossfit workout",
                    slogan: "Push your limits"   
                },
                {
                    image: "service15-2x.jpg",
                    service: "New gym apparel",
                    slogan: "Look good, feel good"   
                },
                {
                    image: "service6-2x.jpg",
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

.overview {
    width: 70%;
    
    p {
        font-size: 1.5em;
        text-align: center;
    }

    .user {
        display: flex;
        justify-content: center;
        align-content:center;

        img {
            width: 40px;
            height: 40px;
            border-radius: 50%;
        }

        ul {
            display: flex;
            list-style: none;
            justify-content: center;
            font-size: .8em;

            li {
                margin: 5px;
               
            
                #username {
                    font-weight: bolder;
                }

                #user-city {
                    color: red;
                }
            }
        }
    }

   
}
</style>