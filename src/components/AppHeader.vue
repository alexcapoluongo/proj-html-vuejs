<template>
  
   <header class="header">
       <div class="ms-container">
           <div class="logo-header">
               <img src="../assets/img/logo.png" alt="">
           </div>
           <div class="menu">
               <ul>
                    <li><a href=""> Home </a></li>
                    <li><a href=""> Services </a></li>
                    <li><a href=""> About </a></li>
                    <li><a href=""> Videos </a></li>
                    <li><a href=""> Blog </a></li>
                    <li><a href=""> Store </a> <span class="new">new</span> </li>
                    <li ><a class="schedule" href=""> Schedule a workout </a></li>
                    <li><a href=""> <i class="fa-solid fa-cart-shopping"></i>
                        </a>
                    </li>
                    <li><a href=""> <i class="fas fa-search"></i>
                        </a>
                    </li>

               </ul>
           </div>
       </div>

  </header>

</template>

<script>
export default {
    name: "AppHeader",
    data() {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";


.header {
    width: 100%;
    height: 60px;
    background-color: black;

    .ms-container {
        display: flex;
        justify-content: space-between;

        .logo-header {
            height: 100%;
            line-height: 60px;

            img {
                width: 70%;
                min-width: 150px;
            }
        }

        .menu {
            font-size: .8em;

            ul {
                display: flex;
                list-style: none;
                height: 100%;

                li {
                    margin-left: 20px;
                    height: 100%;
                    display: flex;
                    align-items: center;

                    .schedule {
                        white-space: nowrap; 
                        color:white;
                        background-color: #4154fe;
                        border-radius: 15px;
                        height: 30px;      
                        padding: 15px;      
                        font-size: .8em;
                    }

                    .new {
                        padding-left: 5px;
                        padding-right: 5px;
                        margin-left: 3px;
                        font-size: .8em;
                        background-color: #FEF966;
                        color: black;
                        border-radius: 3px;
                        line-height: 18px;
                    }

                    a {
                        color: #78787a;
                        line-height: 60px;
                        display: flex;
                        align-items: center;



                        i {
                            line-height: 60px;
                        }
                    }
                }
            }
        }
    }
}


</style>