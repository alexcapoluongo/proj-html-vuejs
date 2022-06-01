<template>
  <div>
      <div class="ms-container"> 
            <!-- grid -->
        <div class="row">
            <div v-for="(item,idx) in servicesArray" :key="idx" class="col">      
                <div class="item" :style="{'background-image': 'url(' + require(`../assets/img/${item.image}`) + ')'}">  
                    <div class="text-wrap mx-3">
                        <img src="../assets/img/zigzagwhite1.png" alt="">
                        <h3 class="mb-0">{{ item.service }}</h3>
                        <p>{{ item.slogan }}</p>
                    </div>
                </div> 
            </div>
        </div>

            <!-- user-overview -->
        <div class="overview m-auto mt-5">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora veritatis nam dignissimos. Natus unde vel culpa quae perferendis fugit saepe recusandae, qui repudiandae necessitatibus quia deleniti perspiciatis officia, quod quidem. </p>
            <div class="zigzag text-center">
                <img src="../assets/img/zigzagyellow1.png" alt="">
            </div>
            
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
                    image: "box1-2x.jpg",
                    service: "New gym apparel",
                    slogan: "Look good, feel good"   
                },
                {
                    image: "box3-2x.jpg",
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

.col {
    margin-top: -40px;
}

.item {
    height: 300px;
    width: 300px;
    margin: auto;
    display: flex;
    justify-content: flex-end;
    flex-direction: column;
    background-size: cover;
    transition: 1s;
    position: relative;
    overflow: hidden;


    &:hover {
       border-bottom-right-radius: 25px;
    }
    //overlay 
    &:after {
    content: '';
    position: absolute;
    width: 100%; height:100%;
    top:0; left:0;
    background:linear-gradient(180deg, rgba(0, 0, 0, .2) 10%, rgba(0, 0, 0, .9) 100%);
    opacity: .5;  
    }

    .text-wrap {
        height: 100px;
        width: 100%;
        z-index:999;

        img {
            width: 40px;
        }

        .zigzag {
            background-color: white;
        }

        h3 {
            color:white;
            font-size: 1.5em;
        }

        p {
            color: $yellow;
        }
    }
}

.overview {
    width: 70%;
    
    p {
        font-size: 1.5em;
        text-align: center;
        color: white;
    }

    .zigzag {
        margin: 0 auto;
        width:40px;        
        
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
            margin-bottom: 100px;

            li {
                margin: 5px;
               
            
                #username {
                    font-weight: bolder;
                    color: white;
                }

                #user-city {
                    color: $jumbo;
                }
            }
        }
    }

   
}
</style>