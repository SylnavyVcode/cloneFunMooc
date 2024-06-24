<template>
  <div>
    <div class="mx-2 md:mx-36">
      <TheNavbarPage></TheNavbarPage>
    </div>
    <TheAccueilPage></TheAccueilPage>
    <TheFooterPage></TheFooterPage>
  </div>
</template>
<script>
import TheNavbarPage from "../navbar/TheNavbarPage.vue";
import TheAccueilPage from "./accueil/TheAccueilPage.vue";
import TheFooterPage from "../footer/TheFooterPage.vue";
export default {
  components: { TheNavbarPage, TheAccueilPage, TheFooterPage },
};
</script>
<style></style>
