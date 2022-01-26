<template>
  <div>
    {{products}}
  </div>
</template>

<script>
export default {
  name: "product1",
  data() {
    return {
      products: []
    }
  },
  async created() {
    const response = await this.$axios.get('/products');
    console.log(response);
    this.products = response.data;
  }
}
</script>

<style scoped>

</style>
