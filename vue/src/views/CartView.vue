<script>
import MenuView from './MenuView.vue';
</script>
<!--
<template>
  <MenuView></MenuView>
  <div v-if="page === cart">
    <h1>Menu</h1>
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
-->