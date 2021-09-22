<template>
  <section :style="whenPrintBreakPage?{pageBreakBefore: 'always'}:{}">
    <slot name="title" />
    <main>
      <slot/>
    </main>
  </section>
</template>

<script>

export default {
  name: "Section",
  props: {
    whenPrintBreakPage: {
      default: false,
      type: Boolean
    }
  }
}

</script>

<style scoped>
section{
  text-align: start;
}
aside {
  width: 150px;
  text-align: end;
}
</style>