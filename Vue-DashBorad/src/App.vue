<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  created() {
    // const api = `${process.env.APIPATH}/api/${process.env.CUSTOMPATH}'`;
    // console.log(api);
    // this.$http.get(api).then(response => {
    //   console.log(response.data);
    // });
  }
};
</script>

<style lang="scss">
// @import "~bootstrap/scss/bootstrap";
@import "./assets/all"

</style>
