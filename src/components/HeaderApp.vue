<template>
    <div class="container">
        <header class="d-flex justify-content-between align-items-center my-4">
      <img src="../assets/images/dc-logo.png" alt="Logo">
      <NavBar />
    </header>
    </div>
  </template>
  
  <script>
  import NavBar from './header/NavBar.vue'
  export default {
    name: 'HeaderApp',
    components: {
      NavBar
    }
  
  }
  </script>
  
  <style lang="scss" scoped>


  </style>