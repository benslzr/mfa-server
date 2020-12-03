<template>
    <div>
      <b-navbar toggleable="lg" type="dark" variant="dark">
          <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
        <b-nav-item to="/idp/logout">Logout: testUser</b-nav-item>
        <b-nav-item to="/support">Help</b-nav-item>
        <b-nav-item to="/about">About</b-nav-item>
      </b-navbar-nav>
      </b-navbar>
</div>
</template>

<style lang="scss" scoped>
#nav a.router-link-exact-active{
    color: #e32626;
  }
</style>