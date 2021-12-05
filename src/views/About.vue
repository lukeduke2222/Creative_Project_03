<template>
  <div class="about">

    <h1 class="section">Company Overview</h1>
    <hr>

    <div class="wrap">
      <div class="stats">
        <div class="stat">
          <h3><u>Founded</u></h3>
          <h1>2014</h1>
        </div>
        <hr class="short">
        <div class="stat">
          <h3><u>Status</u></h3>
          <h1>Private</h1>
        </div>
        <hr class="short">
        <div class="stat">
          <h3><u>Employees</u></h3>
          <h1>100</h1>
        </div>
        <hr class="short">
        <div class="stat">
          <h3><u>Latest Deal Type</u></h3>
          <h1>Seed</h1>
        </div>
      </div>

      <div class="stats">
        <div class="stat-long">
          <h3><u>Latest Deal Amount</u></h3>
          <h1>$3.88M</h1>
        </div>
        <hr class="short">
        <div class="stat">
          <h3><u>Investors</u></h3>
          <h1>79</h1>
        </div>
      </div>
    </div>

    <hr>
    <h1 class="section">General Information</h1>
    <h4 class="section"> Operator of a creative studio intended to offer image design, animation, and effects for visual communications. The company's creative studio offers high-rated visuals, special expertise, and experience, and offers services such as visual asset strategy, animation, digital images, visual effects, post-production, and other similar services, enabling clients to get access to video and animation services.</h4>

  </div>
</template>

<script>
  export default {
    name: "Employees",

  };
</script>

<style scoped>
  .section {
    padding: 40px;
  }

  .stats {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }

  .stat {
    display: flex;
    flex-direction: column;
    height: 150px;

    /* background-color: blue; */
    width: 220px;
  }

  .stat-long {
    display: flex;
    flex-direction: column;
    height: 150px;

    /* background-color: blue; */
    width: 300px;
  }

  .wrap {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 30px;
  }

  .about {
    max-width: 1000px;
    margin: auto;

  }
  .short {
    height: 70px;
    align-self: center;
  }
  hr {
    max-width: 500px;
  }
</style>
