<script setup>
import NavBar from './components/icons/NavBar.vue'
import Footer from './components/icons/Footer.vue'
import Boolean from './components/icons/Boolean.vue'
import ListOfElements from './components/icons/ListOfElements.vue'

</script>


<template>
  <h1>Ironhack Basic Vue.js</h1>
  
  <NavBar> </NavBar>

  <p class="number"> 2 + 2 = {{ 2 + 2 }}</p>

  <Boolean> </Boolean>

  <ListOfElements> </ListOfElements>

  <Footer> </Footer>  
</template>



<style>
body {
  text-align: center;
}
h1 {
  font-family: Arial, Helvetica, sans-serif;
  margin-top: 30px;
  margin-bottom: 60px; 
}
.number {
  font-size: larger;
  background-color: yellowgreen;
  margin: 40px 0px;
  padding: 10px;
}
</style>
