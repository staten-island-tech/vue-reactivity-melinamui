<script>
import TheSushi from '../components/TheSushi.vue';
</script>

<template>
  <TheSushi></TheSushi>
  <h2>{{ cart.length }} in Cart</h2>
  <div v-if="view === 'cart'">
    <h1>Your Cart</h1>
    <div class="menu">
      <div v-for="menu in cart" :key="menu.name">
        {{ menu.name }}
        <img :src="menu.image" />
        <div>{{ menu.cost }}</div>
        <button v-on:click="removefromcart(menu)">Remove from Cart</button>
      </div>
    </div>
  </div>
</template>