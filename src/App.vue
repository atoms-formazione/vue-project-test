<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import MyComponentPietroS from "./components/MyComponentPietroS.vue";
import RandomComponent from "./components/RandomComponent.vue";
</script>

<template>
  <header>
    <img
      alt="Vue logo"
      class="logo"
      src="https://d16u9y6cg00afk.cloudfront.net/Linobanfi/4792707.512.webp"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <HelloWorld msg="You didn't do it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
      <MyComponentSimoneVue></MyComponentSimoneVue>
    </div>
  </header>
  <RouterView />
  <body>
    <h11 class="g2">@RandomComponent</h11>
    <MyComponentPietroS></MyComponentPietroS>
  </body>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
  body .g2{
    background-color: whitesmoke;
  }
}
</style>
