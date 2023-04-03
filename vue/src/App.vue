<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <h1>Menu</h1>
  <div>
  <div v-for="menu in menu"
  :key="menu.name">
  {{ menu.name }}
  </div>
</div>
</template>

<script>
export default {
  name: "App",
  data: () => {
  return {
    menu : [
{
  name: 'Salmon Maki',
  image: '../images/salmon roll.jpg'
},
{
  name: 'Tuna Maki',
  image: '../images/tuna roll.jpg'
},
{
  name: 'Tuna Nigiri',
  image: '../images/tuna roll.jpg'
},
{ name: 'Tamago Nigiri', image: '../images/tamago nigiri.jpg' },
{
  name: 'Shrimp Nigiri',
  image: '../images/shrimp nigiri.jpg'
},
{
  name: 'Roe Nigiri',
  image: '../images/roe .jpg'
},
{
  name: 'Salmon Sashimi',
  image: '../images/salmon sashimi.jpg'
},
{
  name: 'Tuna Sashimi',
  image: '../images/tuna sashimi.jpg'
},
{
  name: 'Tamago',
  image: '../images/tamago .jpg'
},
{
  name: 'Salmon Uramaki',
  image: '../images/salmon uramaki.jpg'
},
{
  name: 'Shrimp Uramki',
  image: '../images/shrimp uramaki.jpg'
},
{
  name: 'Avocado and Salmon Temaki',
  image: '../images/avocade and salmon temaki.jpg'
},
{
  name: 'Tuna Temaki',
  image: '../images/tuna hand roll.jpg'
}
]
  }
}}
</script>



<!--
<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
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
}
</style>
-->
