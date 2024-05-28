<template>
  <main class="mx-36">
    <!-- Main navigation container -->
    <nav
      class="relative flex w-full flex-wrap items-center justify-between bg-zinc-50 py-2 shadow-dark-mild dark:bg-neutral-700 lg:py-4"
      data-twe-navbar-ref
    >
      <div class="flex w-full flex-wrap items-center justify-between">
        <div>
          <a class="my-1 flex items-center lg:mb-0 lg:mt-0" href="#">
            <img
              class="h-30 w-48"
              src="../../assets/images/logo-fr.svg"
              alt="TE Logo"
              loading="lazy"
            />
          </a>
        </div>

        <!-- Hamburger button for mobile view -->
        <div>
          <button
            class="border-0 bg-transparent px-2 text-black/50 hover:no-underline hover:shadow-none focus:no-underline focus:shadow-none focus:outline-none focus:ring-0 dark:text-neutral-200 lg:hidden"
            type="button"
            data-twe-collapse-init
            data-twe-target="#navbarSupportedContent4"
            aria-controls="navbarSupportedContent4"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <!-- Hamburger icon -->
            <span
              class="[&>svg]:w-7 [&>svg]:stroke-black/50 dark:[&>svg]:stroke-neutral-200"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
              >
                <path
                  fill-rule="evenodd"
                  d="M3 6.75A.75.75 0 013.75 6h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 6.75zM3 12a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 12zm0 5.25a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75a.75.75 0 01-.75-.75z"
                  clip-rule="evenodd"
                />
              </svg>
            </span>
          </button>

          <!-- Collapsible navbar container -->
          <div
            class="!visible mt-2 hidden flex-grow basis-[100%] items-center lg:mt-0 lg:!flex lg:basis-auto"
            id="navbarSupportedContent4"
            data-twe-collapse-item
          >
            <!-- Left links -->

            <div class="flex justify-end items-center">
              <button
                type="button"
                data-twe-ripple-init
                data-twe-ripple-color="light"
                class="me-3 inline-block rounded-full px-2 py-3 text-xs font-medium uppercase leading-normal text-black"
              >
                INSCRIPTION
              </button>
              <button
                type="button"
                data-twe-ripple-init
                data-twe-ripple-color="light"
                class="me-3 flex rounded-full bg-red-600 px-6 py-3 text-xs font-medium uppercase leading-normal text-white transition duration-150 ease-in-out"
              >
                <span
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke-width="1.5"
                    stroke="currentColor"
                    class="size-6 me-2"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M17.982 18.725A7.488 7.488 0 0 0 12 15.75a7.488 7.488 0 0 0-5.982 2.975m11.963 0a9 9 0 1 0-11.963 0m11.963 0A8.966 8.966 0 0 1 12 21a8.966 8.966 0 0 1-5.982-2.275M15 9.75a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z"
                    />
                  </svg>
                </span>
                <span class="my-auto">CONNEXION</span>
              </button>
              <button
                type="button"
                data-twe-ripple-init
                data-twe-ripple-color="light"
                class="me-3 inline-block rounded-full bg-red-600 px-6 py-3 text-xs font-medium uppercase leading-normal text-white transition duration-150 ease-in-out"
              >
                FAQ
              </button>
              <div class="text-dark">
                <select name="" id="">
                  <option selected value="fr">Français</option>
                  <option value="en">Anglais</option>
                </select>
              </div>
              <!-- <button
              type="button"
              data-twe-ripple-init
              data-twe-ripple-color="light"
              class="me-3 inline-block rounded bg-neutral-800 px-3 py-2.5 text-xs font-medium uppercase leading-normal text-neutral-50 shadow-dark-3 transition duration-150 ease-in-out hover:bg-neutral-700 hover:shadow-dark-2 focus:bg-neutral-700 focus:shadow-dark-2 focus:outline-none focus:ring-0 active:bg-neutral-900 active:shadow-dark-2 motion-reduce:transition-none dark:shadow-black/30 dark:hover:shadow-dark-strong dark:focus:shadow-dark-strong dark:active:shadow-dark-strong"
            >
              <span class="[&>svg]:w-4">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
                  />
                </svg>
              </span>
            </button> -->
            </div>
          </div>
        </div>
      </div>
      <div
        class="!visible mt-2 hidden flex-grow basis-[100%] items-center lg:mt-0 lg:!flex lg:basis-auto"
      >
        <!-- Main navigation container -->
        <nav
          class="relative flex w-full flex-wrap items-center justify-between bg-zinc-50 py-2 shadow-dark-mild dark:bg-neutral-700 lg:py-4"
        >
          <div class="flex w-full flex-wrap items-center justify-between px-3">
            <nav class="w-full rounded-md" aria-label="breadcrumb">
              <ol class="list-reset ms-2 flex">
                <li class="hover: border-blue-800 hover:border-b-8 pb-3">
                  <a
                    href="#"
                    class="text-black mx-2 font-semibold transition duration-200 hover: border-blue-800 hover:ease-in-out"
                    >Accueil</a
                  >
                </li>

                <li class="hover: border-blue-800 hover:border-b-8 pb-2">
                  <a
                    href="#"
                    class="text-black mx-2 font-semibold transition duration-200 hover: border-blue-800 hover:ease-in-out"
                    >Actualités</a
                  >
                </li>

                <li class="hover: border-blue-800 hover:border-b-8 pb-2">
                  <a
                    href="#"
                    class="text-black mx-2 font-semibold transition duration-200 hover: border-blue-800 hover:ease-in-out"
                    >Cours</a
                  >
                </li>
                <li class="hover: border-blue-800 hover:border-b-8 pb-2">
                  <a
                    href="#"
                    class="text-black mx-2 font-semibold transition duration-200 hover: border-blue-800 hover:ease-in-out"
                    >Etablissements</a
                  >
                </li>
                <li class="hover: border-blue-800 hover:border-b-8 pb-2">
                  <a
                    href="#"
                    class="text-black mx-2 font-semibold transition duration-200 hover: border-blue-800 hover:ease-in-out"
                    >A propos</a
                  >
                </li>
              </ol>
            </nav>
          </div>
        </nav>
      </div>
    </nav>
  </main>
</template>
<script>
export default {};
</script>
<style></style>
