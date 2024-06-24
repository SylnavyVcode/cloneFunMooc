<template>
  <div class="">
    <div class="text-2xl font-semibold flex justify-center items-center mb-6">
      <span>Cours à la Une</span>
    </div>
    <div
      class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6 mx-4 md:mx-0"
    >
      <div
        v-for="(cours, id) in list_cours"
        :key="id"
        class="relative w-full mx-auto bg-white rounded-lg h-[360px] sm:h-[366px] md:h-[376px] shadow-md"
      >
        <img
          class="w-full h-[170px] object-cover rounded-t-lg"
          :src="cours.image"
          alt="Sunset in the mountains"
        />
        <div class="px-6 py-4">
          <div class="font-bold mb-2 text-sm">{{ cours.title }}</div>
          <p
            class="text-[#e51a2d] text-xs flex justify-start items-center"
            :class="{ 'text-[#e51a2d]': status, ' text-black': !status }"
          >
            <span
              ><svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="size-6"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M13.5 21v-7.5a.75.75 0 0 1 .75-.75h3a.75.75 0 0 1 .75.75V21m-4.5 0H2.36m11.14 0H18m0 0h3.64m-1.39 0V9.349M3.75 21V9.349m0 0a3.001 3.001 0 0 0 3.75-.615A2.993 2.993 0 0 0 9.75 9.75c.896 0 1.7-.393 2.25-1.016a2.993 2.993 0 0 0 2.25 1.016c.896 0 1.7-.393 2.25-1.015a3.001 3.001 0 0 0 3.75.614m-16.5 0a3.004 3.004 0 0 1-.621-4.72l1.189-1.19A1.5 1.5 0 0 1 5.378 3h13.243a1.5 1.5 0 0 1 1.06.44l1.19 1.189a3 3 0 0 1-.621 4.72M6.75 18h3.75a.75.75 0 0 0 .75-.75V13.5a.75.75 0 0 0-.75-.75H6.75a.75.75 0 0 0-.75.75v3.75c0 .414.336.75.75.75Z"
                /></svg></span
            ><span class="text-xs">{{ cours.adresse }}</span>
          </p>
        </div>
        <div
          class="bg-[#e51a2d] p-1 text-white bottom-0 absolute w-full rounded-b-lg text-xs"
        >
          <div class="flex">
            <span> </span>
            <span>ouvert à l'inscription</span>
          </div>
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
  </div>
</template>
<script>
import list from "../../cours/cours.json";
export default {
  components: {},
  data() {
    return {
      list_cours: [],
      status: false,
    };
  },
  methods: {
    handleMouseOver(cours) {
      this.status = true;
      console.log(cours);
    },
    // handleMouseOut(){
    //   this.status = false
    // }
  },
  mounted() {
    console.log(list);
    this.list_cours = list.cours;
  },
};
</script>
<style></style>
