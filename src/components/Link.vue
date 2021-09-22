<template>
  <a :href="href" :target="target"><slot/></a>
</template>

<script>
export default {
  name: "Link",
  props:{
    href:String,
    target:String,
  }

}
</script>

<style scoped>
a{
  text-decoration: none;
  border-bottom: 1px solid;
  color: #999;
}
</style>