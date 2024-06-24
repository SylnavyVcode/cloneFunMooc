<template>
  <div>
    <div
      class="bg-cover bg-center bg-[url('src/assets/images/home-intro-funmooc.jpg')]"
    >
      <div class="mx-2 md:mx-36"><TheExploreSection></TheExploreSection></div>
    </div>
    <div class="bg-gradient-to-r from-blue-900 from-10% to-sky-500 to-100% p-3">
      <div class="mx-2 md:mx-36">
        <TheCoursSection></TheCoursSection>
      </div>
    </div>
    <div class="">
      <div class="mx-2 md:mx-36">
        <TheActualitySection></TheActualitySection>
      </div>
    </div>
    <div class="">
      <div class="mx-2 md:mx-36"><TheThemeSection></TheThemeSection></div>
    </div>
    <div class="">
      <div class="mx-2 md:mx-36">
        <TheCreateurSection></TheCreateurSection>
      </div>
    </div>
  </div>
</template>
<script>
import TheExploreSection from "./children/TheExploreSection.vue";
import TheCoursSection from "./children/TheCoursSection.vue";
import TheActualitySection from "./children/TheActualitySection.vue";
import TheThemeSection from "./children/TheThemeSection.vue";
import TheCreateurSection from "./children/TheCreateurSection.vue";

export default {
  components: {
    TheExploreSection,
    TheCoursSection,
    TheActualitySection,
    TheThemeSection,
    TheCreateurSection,
  },
};
</script>
<style></style>
