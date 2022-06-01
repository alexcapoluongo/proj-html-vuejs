<template>
  <div class="store">
      <div class="ms-container text-center mt-5 d-flex align-items-center">
          <div class="text-wrap">
            <h1>"I've failed over and over again in my life. And that is why I succed"</h1>
            <div class="zigzag m-auto mb-4 mt-4"></div>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore dolorem id numquam vel eveniet itaque necessitatibus dolor harum.</p>
            <div class="ms-btn m-auto">Buy Avada today ></div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyStore",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.store {
    width: 100%;
    height: 100%;
    background: rgb(0, 0, 0);
    background: linear-gradient(180deg, rgba(0, 0, 0, .2) 10%, rgba(0, 0, 0, .9) 100%);

}
.ms-btn {
    display: inline;
    padding: 10px;
}
</style>