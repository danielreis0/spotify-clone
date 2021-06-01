<template>
  <div class="flex flex-col my-10 ">
    <div class="text-white w-full px-4 md:px-8  flex flex-col ">
      <div class="flex ">
        <h1
          class="text-xl    font-semibold cursor-pointer hover:underline select-none  "
        >
          {{ data.title }}
        </h1>
      </div>

      <div class=" flex justify-between ">
        <p class="text-sm  text-gray-400 ">
          {{ data.subtitle }}
        </p>
        <p
          class="hidden sm:flex text-sm font-medium  hover:underline cursor-pointer text-gray-400 "
        >
          VER TUDO
        </p>
      </div>
    </div>

    <div class="px-4 md:px-8 mt-3 ">
      <div class="grid grid-cols-footer gap-6">
        <div
          v-for="item in data.cards"
          :key="item.id"
          :class="
            `${
              item.id >= 3
                ? ' hidden  md:flex md:flex-col  '
                : 'flex flex-col  '
            }  transform-gpu group hover:-translate-y-1 justify-center items-center bg-gray-800 text-white rounded-md select-none cursor-pointer transition ease-in-out bg-opacity-30 hover:bg-opacity-80`
          "
        >
          <div
            class="relative h-auto w-full p-4 flex justify-center items-center "
          >
            <img
              :class="
                `${
                  item.type ? ' rounded-full ' : ' rounded-md '
                } w-40 h-auto  bg-green-900   shadow-lg`
              "
              :src="item.img"
              alt=""
            />
            <div
              v-if="item.playable"
              class="absolute flex shadow-xl items-center justify-center bg-green-500 rounded-full h-9 w-9 bottom-10 right-10 opacity-0 transition ease-linear transform-gpu hover:scale-105 hover:bg-green-600 group-hover:opacity-100"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-6 w-6 text-white  "
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

          <div class="  px-4 w-full pb-6">
            <h3 class="text-white text-base font-medium truncate ">
              {{ item.title }}
            </h3>
            <p class="text-gray-400 text-sm truncate ">
              {{
                item.author
                  ? item.author
                  : item.type
                  ? item.type
                  : item.type
                  ? item.user
                  : "De " + item.user
              }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: { data: Object },
};
</script>

<style></style>
