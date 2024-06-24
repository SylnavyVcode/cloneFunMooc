<template>
  <div class="w-full bottom-0 left-0">
    <div class="w-full">
      <img
        class="w-full h-16"
        src="../../assets/images/wave-dark.ad4d56642a16.svg"
        alt=""
      />
    </div>
    <div class="bg-[#232323] px-4 m-0 bottom-0 left-0">
      <div class="bg-[#232323] mb-4">
        <img
          class="w-44"
          src="../../assets/images/logofunMooc-dark.png"
          alt=""
          srcset=""
        />
      </div>
      <div class="md:flex justify-center items-center bg-[#232323]">
        <div class="w-[40%] m-auto">
          <div class="flex justify-right items-center mb-2">
            <select v-model="langue" name="" id="" class="text-center">
              <option value="fr">Français</option>
              <option value="en">Anglais</option>
            </select>
          </div>

          <div class="flex justify-right items-center gap-4">
            <a
              class="rounded-full bg-red-600 text-white w-8 h-8 flex justify-center items-center"
              href=""
              ><span class="[&>svg]:h-5 [&>svg]:w-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 320 512"
                >
                  <path
                    d="M80 299.3V512H196V299.3h86.5l18-97.8H196V166.9c0-51.7 20.3-71.5 72.7-71.5c16.3 0 29.4 .4 37 1.2V7.9C291.4 4 256.4 0 236.2 0C129.3 0 80 50.5 80 159.4v42.1H14v97.8H80z"
                  /></svg></span
            ></a>
            <a
              class="rounded-full bg-red-600 text-white w-8 h-8 flex justify-center items-center"
              href=""
            >
              <!-- X -->
              <span class="[&>svg]:h-5 [&>svg]:w-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 512 512"
                >
                  <path
                    d="M389.2 48h70.6L305.6 224.2 487 464H345L233.7 318.6 106.5 464H35.8L200.7 275.5 26.8 48H172.4L272.9 180.9 389.2 48zM364.4 421.8h39.1L151.1 88h-42L364.4 421.8z"
                  />
                </svg>
              </span>
            </a>
            <a
              class="rounded-full bg-red-600 text-white w-8 h-8 flex justify-center items-center"
              href=""
            >
              <!-- Linkedin -->
              <span class="[&>svg]:h-5 [&>svg]:w-5">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 448 512"
                >
                  <path
                    d="M100.3 448H7.4V148.9h92.9zM53.8 108.1C24.1 108.1 0 83.5 0 53.8a53.8 53.8 0 0 1 107.6 0c0 29.7-24.1 54.3-53.8 54.3zM447.9 448h-92.7V302.4c0-34.7-.7-79.2-48.3-79.2-48.3 0-55.7 37.7-55.7 76.7V448h-92.8V148.9h89.1v40.8h1.3c12.4-23.5 42.7-48.3 87.9-48.3 94 0 111.3 61.9 111.3 142.3V448z"
                  /></svg></span
            ></a>
          </div>
        </div>

        <div class="text-white">
          <h3 class="font-semibold">Apprendre plus</h3>
          <div class="md:grid md:grid-cols-4 md:gap-4 text-sm my-3">
            <div>
              <p class="mb-2">Aide et contact</p>
              <p>A propos de FUN</p>
            </div>
            <div>
              <p class="mb-2">Loi</p>
              <p>Privacy Policy</p>
            </div>
            <div>
              <p class="mb-2">User's charter</p>
              <p>Genral Terms and conditions of use</p>
            </div>
            <div>
              <p class="mb-2">Sitemap</p>
              <p class="m-0 p-0">Cookie management</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-black flex justify-center items-center">
      <div
        class="flex justify-center md:justify-left items-center h-16 text-white"
      >
        <img
          class="m-auto w-24 bg-white rounded-md px-2"
          src="../../assets/images/logo.funMooc1.png"
          alt=""
        />
        <span class="ms-3 text-sm"
          >powered by
          <span class="font-semibold">Sylnavy Valmy MABIKA</span></span
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      langue: "fr",
    };
  },
};
</script>

<style></style>
