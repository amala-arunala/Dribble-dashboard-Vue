<template>
  <div id="app">
    <TheHeader />
    <hr />
    <MainDashboard />
    <TheDetails />
    <ProductService />
    <AboutDribble />
    <hr />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheDetails from "./components/TheDetails.vue";
import TheFooter from "./components/TheFooter.vue";
import AboutDribble from "./components/AboutDribble.vue";
import ProductService from "./components/ProductService.vue";
import MainDashboard from "./components/Dashboard/MainDashboard.vue";

export default {
  components: {
    TheHeader,
    TheDetails,
    ProductService,
    TheFooter,
    AboutDribble,
    MainDashboard,
  },
};
</script>

<style>
#app {
  font-family: "Roboto", sans-serif;
}

hr {
  font-weight: 100;
}
</style>
