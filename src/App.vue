<template>
  <div id="app">
  
  <AppHeader />

  <AppMain />

  <AppFooter />

  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap');
//reset
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-family: 'Roboto Condensed', sans-serif;
}

#app {
   font-family: 'Roboto Condensed', sans-serif;
}
</style>
