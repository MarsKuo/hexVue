<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>

    <button class="btn btn-primary">123124</button>
  </div>
</template>

<script>
export default {
  name: 'App',
  created() {
    const api = `${process.env.APIPATH}/api/${process.env.CUSTOMPATH}/products'`;
    console.log(api);
    this.$http.get(api).then(response => {
      console.log(response.data);
    });
  }
};
</script>

<style lang="scss">
// @import "~bootstrap/scss/bootstrap";
@import "./assets/all"

</style>
