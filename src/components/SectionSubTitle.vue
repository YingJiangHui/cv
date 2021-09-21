<template>
  <header>
    <h3>
      <slot/>
    </h3>
    <ul>
      <li v-for="link of links"><Link href="{{link.href}}">{{link.text}}</Link></li>
    </ul>
  </header>

</template>

<script setup>
import Link from './Link.vue'
</script>

<script>

export default {
  name: "SectionSubTitle",
  props:{
    links:{
      type:Array,
      default: []
    }
  }
}
</script>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

h3 {
  margin-top: .8em;
  color: #666
}

</style>