<template>
  <header>
    <h3>
      <slot/>
    </h3>
    <ul>
      <li v-for="link of links"><Link :href="link.href" :target="'_blank'">{{link.text}}</Link></li>
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
ul>li{
  margin-left: 1em;
  display: inline-block;
}
h3 {
  margin-top: .4em;
  margin-bottom: .4em;
  color: #666
}

</style>