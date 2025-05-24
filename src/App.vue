<script setup>
import Navbar from "./components/NavbarComponent.vue";
import Footer from "./components/FooterComponent.vue";
</script>
<template>
  <div >
    <Navbar />
    <RouterView></RouterView>
    <Footer/>
  </div>

</template>
