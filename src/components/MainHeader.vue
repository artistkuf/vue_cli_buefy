<template>
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
</template>

<script>
export default {
  name: "MainHeader",
};
</script>

<style lang="scss">
.main__navbar {
  a {
    font-weight: 600;
  }
  a:hover {
    background: #bcbcbc;
  }
}
</style>
