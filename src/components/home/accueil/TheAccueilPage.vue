<template>
  <div>
    <div>
      <div class="mx-4 sm:mx-20 md:mx-44 z-10">
        <TheExploreSection></TheExploreSection>
      </div>
    </div>
    <div class="w-full">
      <img
        class="w-full h-16"
        src="../../../assets/images/wave-dark.ad4d56642a16.svg"
        alt=""
      />
    </div>
    <div class="bg-gradient-to-r from-blue-900 from-10% to-sky-500 to-100%">
      <div class="mx-4 sm:mx-20 md:mx-44">
        <TheCoursSection></TheCoursSection>
      </div>
    </div>
    <div class="">
      <div class="mx-4 sm:mx-20 md:mx-44">
        <TheActualitySection></TheActualitySection>
      </div>
    </div>
    <div class="">
      <div class="mx-4 sm:mx-20 md:mx-44">
        <TheThemeSection></TheThemeSection>
      </div>
    </div>
    <div class="">
      <div class="mx-4 sm:mx-20 md:mx-44">
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
