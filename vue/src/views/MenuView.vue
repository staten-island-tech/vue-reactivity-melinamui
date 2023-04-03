<!--<script setup>
import TheSushi from '../components/TheSushi.vue';
</script>-->

<template>
  <h2>{{ cart.length }} in Cart</h2>
    <h1>Menu</h1>
    <div class="menu">
      <div v-for="menu in menu" :key="menu.name">
        {{ menu.name }}
        <img :src="menu.image" />
        <div>{{ menu.cost }}</div>
        <button v-on:click="addtocart(menu)">Add to Cart</button>
      </div>
    </div>
</template>

<script>
export default {
  name: "App",
  data: () => {
    return {
      page: "menu",
      cart: [],
      menu: [
        {
          name: 'Salmon Maki',
          image: '../images/salmon roll.jpg',
          cost: "1 Soul",
        },
        {
          name: 'Tuna Maki',
          image: '../images/tuna roll.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Tuna Nigiri',
          image: '../images/tuna roll.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Tamago Nigiri', image: '../images/tamago nigiri.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Shrimp Nigiri',
          image: '../images/shrimp nigiri.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Roe Nigiri',
          image: '../images/roe .jpg',
          cost: "1 Soul"
        },
        {
          name: 'Salmon Sashimi',
          image: '../images/salmon sashimi.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Tuna Sashimi',
          image: '../images/tuna sashimi.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Tamago',
          image: '../images/tamago .jpg',
          cost: "1 Soul"
        },
        {
          name: 'Salmon Uramaki',
          image: '../images/salmon uramaki.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Shrimp Uramki',
          image: '../images/shrimp uramaki.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Avocado and Salmon Temaki',
          image: '../images/avocade and salmon temaki.jpg',
          cost: "1 Soul"
        },
        {
          name: 'Tuna Temaki',
          image: '../images/tuna hand roll.jpg',
          cost: "1 Soul"
        }
      ]
    };
  },
  methods: {
    addtocart(menu) {
      this.cart.push(menu);

    }
  },
  components: {}
};
</script>

<style scoped>
.menu {
  display: flex;
  align-items: center;
  flex-direction: column;
}

img {
  width: 500px;
  height: 500px;
}
</style>


<!--
<template>
  <main>
    <TheSushi/>
  </main>
</template>
-->