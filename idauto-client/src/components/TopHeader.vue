<template>
  <div id="top-navigation">
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="/">ONE PORTAL</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="/">Home</b-nav-item>
        <b-nav-item to="/users">Users</b-nav-item>
        <b-nav-item href="/clients">Clients</b-nav-item>
        <b-nav-item href="/settings">Settings</b-nav-item>
        <b-nav-item to="/support">Help</b-nav-item>
        <b-nav-item to="/about">About</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<style lang="scss" scoped>
#nav a.router-link-exact-active{
    color: #e32626
}

#top-navigation{
  background: #5b6a73;
  margin-bottom: 10px;
}
</style>