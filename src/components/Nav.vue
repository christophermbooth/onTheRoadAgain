<template>
<b-navbar class="p-3 mb-2 bg-warning text-dark" toggleable="lg" type="light">

  <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

  <b-collapse id="nav-collapse" is-nav>
    <b-navbar-nav>
      <b-nav-item href="#">
        <router-link class="app_link" to="/login">Home</router-link>
      </b-nav-item>
      <b-nav-item href="#">
        <router-link class="app_link" to="/newtrip">Create a Trip</router-link>
      </b-nav-item>
      <b-nav-item href="#">
        <router-link class="app_link" to="/profile">My Trips</router-link>
      </b-nav-item>
      <b-nav-item href="#">
        <router-link class="app_link" to="/journal">Journal</router-link>
      </b-nav-item>
    </b-navbar-nav>

    <!-- Right aligned nav items -->
    <b-navbar-nav class="ml-auto">
      <a class="home_sign_in" href="/logout">Logout</a>
    </b-navbar-nav>
  </b-collapse>
</b-navbar>
</template>

<script>
export default {
  name: "Nav",
};
</script>

<style>
.app_link {
  text-decoration: none;
}

b-navbar {
  color:  #2b3e40;
}
</style>
