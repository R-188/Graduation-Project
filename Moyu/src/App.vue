<template>
  <div class="app">
    <Header></Header>
  </div>
  <div class="section">
    <Shop></Shop>
  </div>
</template>



<script>
import Header from "./components/index/index.vue"

import Shop from "./components/index/Shop.vue"

export default {
  name: "app",
  components: {
    Header,
    Shop
    }
}
</script>