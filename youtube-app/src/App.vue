<template>
  <header class="header">
    <div class="header-wrapper">
      <nav class="links">
        <router-link class="link" to="/">Home</router-link>
        <div class="links">
          <router-link class="link" to="/login">Login</router-link>
          <router-link class="link" to="/admin">Admin</router-link>
          <router-link class="link" to="/favourite">Favourite</router-link>
        </div>
      </nav>
    </div>
  </header>
  <router-view/>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.link.router-link-exact-active {
  color: #c73a0f;
}

.links{
  display: flex;
  justify-content: space-between;
}

.link {
  margin-right: 1.25rem;
  padding: 1.25rem 0;
  text-decoration: none;
  color: #0c0c14;
}

.link:last-child {
  margin-right: 0;
}

.header {
  background-color: rgba(229, 229, 229, 1);
  width: 100%;
}

.header-wrapper {
  max-width: 90rem;
  margin: 0 auto;
  padding: 0 1.25rem;
}

</style>
