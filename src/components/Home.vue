<template>
  <div>
    <h1>Hello From Home Component</h1>
    <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String
  }
}
</script>

<style scoped>

</style>