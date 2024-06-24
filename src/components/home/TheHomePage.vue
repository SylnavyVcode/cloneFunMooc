<template>
  <div class="relative">
    <div>
      <div
        v-if="page == 'home'"
        class="h-screen mt-[-20px] absolute inset-0 bg-cover bg-center bg-[url('src/assets/images/home-intro-funmooc.jpg')]"
      ></div>
      <div class="mx-4 sm:mx-20 md:mx-44">
        <TheNavbarPage @goPage="pageCurrent"></TheNavbarPage>
      </div>
      <div class="relative z-10">
        <TheAccueilPage></TheAccueilPage>
      </div>
    </div>
    <div v-if="page != 'home'">
      <!-- <div
        v-if="page == 'home'"
        class="bg-cover bg-center bg-[url('src/assets/images/home-intro-funmooc.jpg')]"
      ></div> -->
      <div class="mx-4 sm:mx-20 md:mx-44">
        <TheNavbarPage @goPage="pageCurrent"></TheNavbarPage>
      </div>

      <TheAccueilPage></TheAccueilPage>
    </div>
  </div>
  <TheFooterPage></TheFooterPage>
</template>
<script>
import TheNavbarPage from "../navbar/TheNavbarPage.vue";
import TheAccueilPage from "./accueil/TheAccueilPage.vue";
import TheFooterPage from "../footer/TheFooterPage.vue";
export default {
  components: { TheNavbarPage, TheAccueilPage, TheFooterPage },
  data() {
    return {
      page: "",
    };
  },
  methods: {
    pageCurrent(page) {
      console.log("current page ======", page);
      this.page = page;
    },
  },
};
</script>
<style></style>
