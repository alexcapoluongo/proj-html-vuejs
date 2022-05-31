<template>
  <div>
      <div class="ms-container">
          <div class="title-wrap d-flex justify-content-between align-items-center mt-5">
            <h4>Featured playlists</h4>
            <a href="">View all videos ></a>
          </div>

        <div class="container">
            <div class="row d-flex justify-content-between">
                <div class="item col-4">
                    <img src="../assets/img/video2-2x.jpg" alt="">
                </div>
                <div class="item col-4">
                    <img src="" alt="">
                </div>
                <div class="item col-4">
                    <img src="" alt="">
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyVideos",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.item {
    border: 1px solid black;
    width: 30%;

    img {
        width: 100%;
    }
}

</style>