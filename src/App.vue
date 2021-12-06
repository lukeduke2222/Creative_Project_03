<template>
  <div id="app">
    <div id="nav">
      <img class="logo-img" alt="COmpany Logo Here" src="/comp_logo.png" width="500px"/>
      <div class="">
        <router-link to="/">Home</router-link> |
        <router-link to="/employees">Employees</router-link> |
        <router-link to="/about">About</router-link>

      </div>
    </div>
    <router-view />
    <div class="footer">
      <p class="left center">  <a href="https://github.com/lukeduke2222/Creative_Project_03"><img alt="GitPage" src="/git-logo.png" width="70px"/></a> </p>
    </div>
  </div>
</template>

<style>
.footer {
  width: 100%;
  height: 100px;
  background-color: #bebebe !important;

}

.logo-img {
  align-self: center;
  margin-bottom: 20px;
  padding-right: 60px;
}

.left {
  padding-top: 30px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  display: flex;
  flex-direction: column;
  background-color: #bebebe !important;

}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
