<template>
  <section class="w-full">
    <div class="md:w-2/3 mb-6 md:mb-28">
      <h1 class="text-4xl font-semibold">
        <span class="text-red-600">Se former</span> en liberté
      </h1>
      <h4 class="text-xl">
        Des cours en ligne pour découvrir, apprendre, progresser et réussir
      </h4>
    </div>
    <div>
      <form>
        <div class="mb-6">
          <label for="search_cours" class="text-lg font-bold"
            >Chercher dans nos cours</label
          >
        </div>
        <div class="block md:flex justify-center items-center w-full">
          <div class="relative w-full">
            <input
              type="search"
              id="search_cours"
              class="block p-2.5 w-full z-20 text-sm text-white rounded-s-full rounded-e-full border"
              placeholder="Recherche de cours"
              required
            />
            <button
              type="submit"
              class="absolute top-0 end-0 p-2.5 h-full text-sm font-medium text-white bg-[#e51a2d] rounded-e-full border focus:ring-4"
            >
              <svg
                class="w-4 h-4"
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 20 20"
              >
                <path
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"
                />
              </svg>
            </button>
          </div>
          <div class="flex justify-center items-center my-3 w-full">
            <button
              class="text-xs border-0 pointer p-3 px-4 rounded-full text-white bg-[#e51a2d] hover:no-underline hover:shadow-none focus:no-underline focus:shadow-none focus:outline-none focus:ring-0"
            >
              Explorer notre catalogie ->
            </button>
          </div>
        </div>
      </form>
    </div>
  </section>
</template>
<script>
export default {
  components: {},
};
</script>
<style></style>
