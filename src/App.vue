<template>
  <div id="app">
    <!--  <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <b-navbar class="is-light main__navbar">
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img src="@/assets/logo.png" alt="Vuejs logo" />
        </b-navbar-item>
      </template>
      <template slot="start">
        <b-navbar-item tag="router-link" :to="{ path: '/' }"> Home </b-navbar-item>
        <b-navbar-item tag="router-link" :to="{ path: '/about' }"> About </b-navbar-item>
      </template>
    </b-navbar>
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap");
#app {
  font-family: "Roboto Condensed", sans-serif;
  font-weight: 100;
  text-align: center;
  color: #2c3e50;
}
.main__navbar {
  a {
    font-weight: 600;
  }
  a:hover {
    background: #bcbcbc;
  }
}
</style>
