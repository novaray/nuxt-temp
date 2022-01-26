<template>
  <div>
    {{ products }}
  </div>
</template>

<script>
export default {
  name: "product2",
  components: {},
  async asyncData( {$axios} ) {
    const response = await $axios.get('/products');
    const products = response.data;
    return { products };
  },
}
</script>

<style scoped>

</style>
