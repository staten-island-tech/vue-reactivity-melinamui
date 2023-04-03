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