<template>
  
   <header class="header">
       <div class="ms-container">
           <div class="logo-header">
               <img src="../assets/img/logo.png" alt="">
           </div>
           <div class="menu">
               <ul>
                    <li><a class="active" href="#hero-banner"> Home </a></li>
                    <li><a href="#services"> Services </a></li>
                    <li><a href="#about"> About </a></li>
                    <li><a href="#videos"> Videos </a></li>
                    <li><a href="#blog"> Blog </a></li>
                    <li><a href="#store"> Store </a> <span class="new">new</span> </li>
                    <li ><a class="schedule" href="#schedule"> Schedule a workout </a></li>
                    <li><a href="#shop"> <i class="fa-solid fa-cart-shopping"></i>
                        </a>
                    </li>
                    <li><a href="#search"> <i class="fas fa-search"></i>
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
    position: fixed;
    top: 0;
    right: 0;

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

                        &:hover {
                            background-color: #ec5a57;
                        }
                    }

                    .active {
                        color: white;
                    }

                    .new {
                        padding-left: 5px;
                        padding-right: 5px;
                        margin-left: 3px;
                        font-size: .8em;
                        background-color: $yellow;
                        color: black;
                        border-radius: 3px;
                        line-height: 18px;
                    }

                    a {
                        color: $jumbo;
                        line-height: 60px;
                        display: flex;
                        align-items: center;

                        &:hover {
                            color: white;
                        }

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