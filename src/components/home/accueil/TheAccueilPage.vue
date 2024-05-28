<template>
  <div>
    <TheExploreSection></TheExploreSection>
    <TheCoursSection></TheCoursSection>
    <TheActualitySection></TheActualitySection>
    <TheThemeSection></TheThemeSection>
    <TheCreateurSection></TheCreateurSection>
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
