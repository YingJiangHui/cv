<template>
  <p>
    <slot/>
  </p>
</template>

<script>
export default {
  name: "Paragraph",

}
</script>

<style scoped>
p {
  line-height: 1.5;
  margin: 0.3em;
}
</style>