<template>
  <article>
    <slot />
  </article>
</template>

<script>


export default {
  name: "Article"
}
</script>

<style scoped>
article {
  background: #fff;
  width: 21cm;
  padding: 1em;
  text-align: start;
}
</style>