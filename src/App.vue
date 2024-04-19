<template>
  <div id="app">
    <header>
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>|
      <router-link v-if="$auth.isAuthenticated" to="/profile">Profile</router-link>
    </header>
    <div class="container fluid">
      <div class="row">
        <div class="col-md-8 offset-md-2">
          <router-view></router-view>
        </div>
      </div>  

    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style></style>