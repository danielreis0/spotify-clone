<template>
  <div class="mx-4 md:mx-8 flex flex-col  ">
    <div class=" my-4">
      <h1 class="text-white font-extrabold text-3xl">Boa noite</h1>
    </div>
    <div
      class="mt-2 grid gap-4 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-3"
    >
      <div
        v-for="item in data"
        :key="item.id"
        :class="
          ` ${
            item.id > 4 ? 'hidden xl:flex' : item.id > 2 ? 'hidden md:flex' : ''
          } select-none  group relative flex items-center rounded-md shadow-lg transform-gpu  hover:-translate-y-1 cursor-pointer bg-gray-600 bg-opacity-40 transition ease-linear hover:bg-opacity-80`
        "
      >
        <div class=" flex items-center w-full ">
          <img class="shadow w-20 h-20 rounded-l-md" :src="item.img" alt="" />
          <p
            class="mr-4 ml-2 h-auto overflow-ellipsis overflow-hidden ...  text-white font-semibold text-sm"
          >
            {{ item.title }}
          </p>
        </div>

        <div class=" flex h-full ml-auto  mr-4 justify-end items-center   ">
          <div
            class="  flex justify-center items-center rounded-full h-9 w-9 bg-green-500 transition ease-linear opacity-0 hover:bg-green-600 transform-gpu hover:scale-110  group-hover:opacity-100"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-white  "
              viewBox="0 0 20 20"
              fill="currentColor"
            >
              <path
                fill-rule="evenodd"
                d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z"
                clip-rule="evenodd"
              />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    data: Array,
  },
};
</script>

<style></style>
