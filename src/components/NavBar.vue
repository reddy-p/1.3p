<template>
  <nav>
    <!-- Logo on the left -->
    <a class="logo" href="/">
      <img src="favicon.ico" alt="Logo" />
    </a>

    <!-- Navigation items on the right -->
    <div class="navbar-menu">
        <router-link to="/" class="navbar-item">Projects</router-link>
        <router-link to="/about" class="navbar-item">About</router-link>
    </div>
  </nav>
</template>

<style>
/* You can add your custom CSS styles here for the navbar and its components */
nav {
  width: 100%;
  max-height: fit-content;
  padding: 0rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 2px solid #0088ff;
}

.navbar-item {
  color: #0088ff;
  padding: 1rem;
}
</style>
