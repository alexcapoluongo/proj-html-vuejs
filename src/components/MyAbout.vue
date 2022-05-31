<template>
  <div>
      
          <div class="container pt-5">
              <div class="row">
                  <div class="col-6">
                      <img class="video-img" src="../assets/img/service15-2x.jpg" alt="">
                  </div>
                  <div class="col-6">
                      <section class="about-text mt-5">
                            <p>Tune up your workout</p>
                            <h1>The best health & fitness advice online</h1>
                            <div class="youtube-channel mt-3 mb-3">
                                <img class="mx-2" src="../assets/img/unnamed.jpg" alt="">
                                <div class="yt-user">
                                    <div class="name-channel mb-1">ThemeFusion</div>
                                    <div class="subscribe">
                                        <div class="btn-subscribe">
                                            <i class="fa-brands fa-youtube mx-1"></i>YouTube
                                            <div>999+</div>
                                        </div>
                                        
                                    </div>
                                </div>
                            </div>
                            <p class="mb-4">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Perspiciatis qui aliquid necessitatibus libero.
                            </p>
                            <div class="ms-btn btn-red">
                                <i class="fa-brands fa-youtube mx-1"></i>
                                <a href="">Visit my Youtube Channel</a> 
                            </div>
                            
                      </section>
                  </div>
              </div>
          </div>
      
 </div>
</template>

<script>
export default {
    name: "MyAbout",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.video-img {
    width: 80%;
    border-bottom-right-radius: 25px;
    margin-top: -80px;
    border-bottom-right-radius: 25px;

}

.row > * {
    padding-left: 0;
}

.about-text {

    width: 80%;
    margin: 0 auto;

    p:first-child {
        color:blue;
    }

    .youtube-channel {
        display:flex;

        img {
            width: 40px;
            height:40px;
        }

        .name-channel {
            font-size: .7em;
            color: $jumbo;
        }

        .btn-subscribe {
            background-color: red;
            color: white;
            font-size: .7em;
            padding-left: 5px;
            
            &:hover {
                background-color: #EB5252;
            }

            div {
                background-color: white;
                color: $jumbo;
                display: inline-block;
                border: 1px solid $jumbo;
                border-left: transparent;
                padding-right: 5px;
                padding-left: 5px;
            }
        }

    }
    p {
        color: $jumbo;
    }


    .btn-red {
        display: inline;
        color: white;

        &:hover {
                background-color: #EB5252;
            }

        a {
            color: white;
        }
    }

}

</style>