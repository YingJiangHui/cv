<template>
  <h2>
    <slot/>
  </h2>
  <Line />
</template>
<script setup>
import Line from './Line.vue'

</script>

<script>
export default {
  name: "SectionTitle",
  props: {
    color: {
      type: String,
    }
  }
}
</script>

<style scoped>
h2 {
  margin-top: .8em;
}
</style>