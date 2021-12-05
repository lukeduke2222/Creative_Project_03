<template>
  <div id="app">
    <div id="nav">
      <img alt="COmpany Logo Here" src="/assets/logo.png" />
      <div class="">
        <router-link to="/">Home</router-link> |
        <router-link to="/employees">Employees</router-link> |
        <router-link to="/about">About</router-link>

      </div>
    </div>
    <router-view />
    <div class="footer">
      <p>this is the footer</p>
    </div>
  </div>
</template>

<style>
.footer {
  width: 100%;
  height: 100px;
  background-color: #bebebe !important;
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
