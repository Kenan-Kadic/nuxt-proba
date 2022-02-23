<template>
  <v-container>
  <Navbar></Navbar>
    <home></home>
  </v-container>
</template>

<script>
import Home from"./home";
import Navbar from "~/components/Navbar";
export default {
  components: {Navbar, Home}
}
</script>
