<template>
<div class="wrapper">
  <div class="employees">
    <div class="employee" v-for="employee in employees" :key="employee.id">
      <div class="info">
        <h1>{{employee.first_name + employee.last_name}}</h1>
        <p>{{employee.city}}</p>
      </div>
      <div class="image">
        <img :src="employee.avatar">
      </div>
      <div class="price">
        <h2>{{employee.phone_number}}</h2>
        <!-- <button class="auto" @click="addToCart(product.id-1)">Add to Cart</button> -->
      </div>
    </div>
  </div>
</div>
</template>

<script>
//import cart from "../main.js";

export default {
  name: 'EmployeeList',
  props: {
    employees: Array,
  },

  methods: {

  },
}

</script>

<style scoped>
  .employees {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  .employee {
    width: 300px;
    margin-bottom: 50px;
    padding-bottom: 30px;
    background-color: #eeeeee;
    border: solid #666666 1px;
    border-radius: 5px;
  }
</style>
