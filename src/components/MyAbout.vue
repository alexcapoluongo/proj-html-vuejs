<template>
  <div>
      <div class="ms-container pt-5">
          <div class="container">
              <div class="row">
                  <div class="col-6">
                      <img class="video-img" src="../assets/img/service15-2x.jpg" alt="">
                  </div>
                  <div class="col-6">
                      <section class="about-text">
                            <p>Tune up your workout</p>
                            <h1>The best health & fitness advice online</h1>
                            <div class="youtube-channel">
                                <img src="" alt="">
                                <div class="yt-user">
                                    <div class="name-channel"></div>
                                    <div class="subscribe">
                                        <div class="btn-subscribe"></div>
                                        <div class="number-subscribe"></div>
                                    </div>
                                </div>
                                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Perspiciatis qui aliquid necessitatibus ducimus minima modi omnis est dolorum, quis tempora libero magnam exercitationem explicabo voluptatem praesentium quas repellendus optio distinctio?
                                </p>
                                <div class="ms-btn">Visit my Youtube Channel</div>
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

    p {
        color: gray;
    }
}

</style>