<template>
  <div>
      <div class="ms-container pt-5">
          <div class="container">
              <div class="row">
                  <div class="col-6">
                      <img class="video-img" src="../assets/img/service15-2x.jpg" alt="">
                  </div>
                  <div class="col-6">
                      <section class="about-text mt-5">
                            <p>Tune up your workout</p>
                            <h1>The best health & fitness advice online</h1>
                            <div class="youtube-channel mt-3 mb-3">
                                <img src="../assets/img/unnamed.jpg" alt="">
                                <div class="yt-user">
                                    <div class="name-channel">ThemeFusion</div>
                                    <div class="subscribe">
                                        <div class="btn-subscribe">
                                            <i class="fa-brands fa-youtube"></i>YouTube
                                            <div>999+</div>
                                        </div>
                                        
                                    </div>
                                </div>
                            </div>
                            <p class="mb-4">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Perspiciatis qui aliquid necessitatibus ducimus minima modi omnis est dolorum, quis tempora libero magnam exercitationem explicabo voluptatem praesentium quas repellendus optio distinctio?
                            </p>
                            <div class="ms-btn btn-red">
                                <i class="fa-brands fa-youtube"></i>
                                Visit my Youtube Channel
                            </div>
                            
                      </section>
                  </div>
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
    width: 100%;
}

.row > * {
    padding-left: 0;
}

.about-text {

    p:first-child {
        color:blue;
    }

    .youtube-channel {
        display:flex;

        img {
            width: 30px;
            height:30px;
        }

        .name-channel {
            font-size: .8em;
            color: $jumbo;
        }

        .btn-subscribe {
            background-color: red;
            color: white;
            font-size: .7em;
            padding-left: 5px;
            

            div {
                background-color: white;
                color: $jumbo;
                display: inline-block;
                border: 1px solid $jumbo;
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
        color: white
    }

}

</style>