<template>
  <div class="container">
    <slot />
  </div>
</template>


<script>
export default {
  name: "HeaderItem",
  data() {
    return {
    };
  },
};
</script>

<style scoped>
.container {
  color: #ddd;
}
.container:hover{
  color: #aaa;
  box-shadow: 0px -2px 0px aliceblue inset;
}
</style>