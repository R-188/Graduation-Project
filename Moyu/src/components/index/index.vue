<template>
  <nav class="header">
    <div class="container mx-auto">
      <div class="left-grid">
        <HeaderItem>Icon</HeaderItem>
      </div>
      <div class="right-grid">
        <HeaderItem>Home</HeaderItem>
        <HeaderItem>About</HeaderItem>
      </div>
    </div>
  </nav>
</template>


<script>
import HeaderItem from './HeaderItem.vue'

export default {
  name: 'Header',
  components: {
    HeaderItem
  },
  data() {
    return {}
  }
}
</script>

<style scoped>
.container {
  display: flex;
  background-color: rgb(243, 221, 20);
  flex-direction: row;
  justify-content: space-between;
  padding: 10px 20px;
  border-radius: 0.25em;
  width: 100%;
}
.left-grid {
  display: flex;
  flex-direction: row;
}
.right-grid {
  display: flex;
  flex-direction: row;
}
</style>