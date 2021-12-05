<template>
  <div class="home">
    <!-- <img src="../assets/logo.png"> -->
    <h1 class="item">Welcome to the Fast Banana Family!</h1>
    <hr>
    <div class="item">
      <h2>What we do</h2>
      <h3>We deal with online marketing in order to make <i>your</i> business a success</h3>
    </div>
    <hr>
    <div class="item">
      <h2>How We do It</h2>
      <h3>We will customize your webpages and make a execute an advertizing campaign according to your specific needs.
      We have several plans to fit your needs best, ranging from our personal plans, small-business plans, to our
      coorporate plans.</h3>
    </div>
    <hr>
    <div class="item">
      <h1>Contact us today for a free estimate!</h1>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  // components: {
  //   HelloWorld,
  // },
};
</script>

<style scoped>
  .item {
    padding: 40px;
  }
  hr {
    max-width: 500px;
  }
</style>
