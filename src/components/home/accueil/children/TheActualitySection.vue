<template>
  <div class="text-2xl font-semibold flex justify-center items-center mb-6">
    <span>Actualités</span>
  </div>
  <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mx-8 md:mx-0">
    <div v-for="(actu, id) in list_actu" :key="id" class="w-full mx-auto">
      <span :class="{ 'text-red-700': status, ' text-black': !tatus }">{{
        actu.date
      }}</span>
      <img
        class="w-full rounded-lg"
        :src="actu.image"
        alt="Sunset in the mountains"
      />
      <div class="px-6 py-4">
        <div class="font-bold text-xl mb-2">{{ actu.title }}</div>
        <p
          class="text-gray-700 text-base"
          :class="{ 'text-red-700': status, ' text-black': !tatus }"
        >
          {{ actu.message }}
        </p>
      </div>
      <!-- <div class="px-6 pt-4 pb-2">
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2"
          >#photography</span
        >
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2"
          >#travel</span
        >
        <span
          class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2"
          >#winter</span
        >
      </div> -->
    </div>
  </div>
</template>
<script>
import list from "../../actuality/actuality.json";
export default {
  components: {},
  data() {
    return {
      list_actu: [],
      status: false,
    };
  },
  methods: {
    handleMouseOver(actu) {
      this.status = true;
      console.log(actu);
    },
    // handleMouseOut(){
    //   this.status = false
    // }
  },
  mounted() {
    console.log(list);
    this.list_actu = list.actu;
  },
};
</script>
<style></style>
