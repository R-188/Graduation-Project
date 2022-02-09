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
  color: rgb(0, 0, 0);
}
.container:hover{
  color: #aaa;
  box-shadow: 0px -5px 0px rgba(253, 168, 11, 0.787) inset;
}
</style>