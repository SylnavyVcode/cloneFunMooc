<template>
  <div class="pt-4 text-3xl font-bold flex justify-center items-center mb-6">
    <span>Actualités</span>
  </div>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mx-8 md:mx-0 pb-6">
    <div
    @mouseover="sttutTextNews(id)" @mouseout="valueIdNew = null"
      v-for="(actu, id) in list_actu"
      :key="id"
      :class="{
        'mx-auto': true,
        'md:col-span-2': id === 0,
        'pt-12': id === 1
      }"
      class="w-full"
    >
      <span
        class="text-xs px-3"
        :class="{ 'text-[#e51a2d]': valueIdNew == id, 'text-black': valueIdNew != id }"
      >
        {{ actu.date }}
      </span>
      <img
        class="w-full rounded-lg"
        :src="actu.image"
        alt="Sunset in the mountains"
      />
      <div class="p-4">
        <div
          :class="{ 'text-[#e51a2d]': valueIdNew == id, 'text-black': valueIdNew != id }"
          class="font-bold text-xl mb-2"
        >
          {{ actu.title }}
        </div>
        <p class="text-gray-700 text-base">
          {{ actu.message }}
        </p>
      </div>
    </div>
  </div>
  <div class="flex justify-center items-center py-8">
      <button class="rounded-md bg-red-600 text-white pointer font-semibold px-5 text-sm py-3">MORE COURSES</button>
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
      valueIdNew: null,
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
    sttutTextNews(id){
console.log("id >>>>>", id);
this.valueIdNew = id
    }
  },
  mounted() {
    console.log(list);
    this.list_actu = list.actu;
  },
};
</script>
<style></style>
