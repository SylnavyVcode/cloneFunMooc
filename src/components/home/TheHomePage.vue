<template>
  <div class="mx-2 md:mx-36">
    <TheNavbarPage></TheNavbarPage>
    <TheAccueilPage></TheAccueilPage>
  </div>
</template>
<script>
import TheNavbarPage from "../navbar/TheNavbarPage.vue";
import TheAccueilPage from "./accueil/TheAccueilPage.vue";
export default {
  components: { TheNavbarPage, TheAccueilPage },
};
</script>
<style></style>
