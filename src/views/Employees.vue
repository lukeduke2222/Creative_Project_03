<template>
  <div class="employees">
    <!-- <img src="../assets/logo.png"> -->
    <h1>Employees Page</h1>

      <form >
        <input class="search" v-model="searchText" placeholder="Search By Employee Name">
      </form>
      <hr>
    <EmployeeList :employees="employees"/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
import EmployeeList from "../components/EmployeeList.vue"
export default {
  name: "Employees",
  components: {
    EmployeeList
  },
  data() {
    return {
    searchText: '',
    }
  },
  computed: {

    employees() {
      return this.$root.$data.employees.filter(employee =>
        employee.first_name.toLowerCase().search(this.searchText.toLowerCase()) >= 0);
    }
  },
};
</script>

<style scoped>
  hr {
    max-width: 700px;
    margin-bottom: 60px;
  }
  /* .search {
  border: 1px solid #ccc;
  border-radius: 4px;
  width: 50%;
} */

form {
  display: table;
  width: 100%;
}

.search {
  width: 50%;
  height: 40px;
  margin: 50px;
  font-size: 20px;
  text-align: center;
}
</style>
