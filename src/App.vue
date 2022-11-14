<template>
  <div id="app">
    <NavbarComp />
  </div>
</template>

<script>
import NavbarComp from "@/components/Navbar";
export default {
  name: 'App',
  components: {
    NavbarComp

  }
}
</script>

<style>
* {
  margin: 0 !important;
  font-family: 'Roboto', sans-serif;
}
</style>
