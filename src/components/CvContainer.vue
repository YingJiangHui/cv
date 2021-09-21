<template>
  <div class="cv-container">
    <slot/>
  </div>
</template>

<script>
export default {
  name: "CvContainer"
}
</script>

<style scoped>
.cv-container {
  display: flex;
  justify-content: center;
  height: 100%;
  width: 100%;
}
</style>