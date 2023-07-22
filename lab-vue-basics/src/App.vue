<script setup>
import NavBar from './components/icons/NavBar.vue'
import Footer from './components/icons/Footer.vue'


</script>

<template>
  <NavBar> </NavBar>

  <p>Shops are for adults only. Validate you're <input type="number" placeholder="age" {{ age }}> to enjoy or ask you're mom to help you find the best clothing for you!</p>
  <p v-if="age >=14"> It's shopping day! Enjoy our limited edition with a reasonable price!</p>
  <p v-else>It's too early for you to shop.</p>

<!--- 
<h2>Shops Here</h2> 
  <ul>
    <li>Men</li>
    <li>Women</li>
    <li>Kids</li>
  </ul>
  -->
  <Footer> </Footer>
  
</template>


<style>

</style>
