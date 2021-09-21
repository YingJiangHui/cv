<template>
  <section>
    <slot name="title" />
    <main>
      <slot/>
    </main>
  </section>
</template>

<script>

export default {
  name: "Section",
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