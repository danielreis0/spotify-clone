<template>
  <div class="flex flex-col  h-screen sticky top-0">
    <div class="w-16   sm:w-44 md:w-52 lg:w-56 h-screen bg-black">
      <div class="flex flex-col w-full h-full ">
        <div
          class="select-none flex justify-items-center items-center w-full  py-4 mt-2 "
        >
          <img
            src="https://logodownload.org/wp-content/uploads/2016/09/spotify-logo-branca-white.png"
            class="hidden sm:inline-block px-10"
          />
          <img
            src="https://i.imgur.com/bh5LATC.png"
            class="inline-block sm:hidden  px-4"
          />
        </div>
        <div class="w-full ">
          <ul
            class="select-none flex flex-col justify-center items-center px-2 mt-2"
          >
            <li
              v-for="item in items"
              :key="item.key"
              :class="
                `${
                  selectedItem == item.key
                    ? 'bg-gray-800  opacity-100'
                    : 'bg-black opacity-60 hover:opacity-100'
                } w-full flex justify-start items-center h-10 rounded-md  text-white cursor-pointer  transition duration-300 ease-in-out`
              "
              @click="selectedItem = item.key"
            >
              <div class="flex items-center mx-auto sm:mx-1">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6 sm:mx-3"
                  :viewBox="item.stroke ? '0 0 24 24' : '0 0 20 20'"
                  :fill="item.stroke ? 'none' : 'currentColor'"
                  :stroke="item.stroke ? 'currentColor' : ''"
                >
                  <path
                    :d="item.svg"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                  />
                </svg>
                <h5 class="hidden sm:inline-flex text-xs font-semibold">
                  {{ item.title }}
                </h5>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedItem: "home",
      items: [
        {
          title: "Início",
          svg:
            "M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6",
          stroke: true,
          key: "home",
        },
        {
          title: "Buscar",
          svg:
            "M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z",
          key: "search",
        },
        {
          title: "Sua biblioteca",
          svg:
            "M2 4a1 1 0 011-1h2a1 1 0 011 1v12a1 1 0 01-1 1H3a1 1 0 01-1-1V4zM8 4a1 1 0 011-1h2a1 1 0 011 1v12a1 1 0 01-1 1H9a1 1 0 01-1-1V4zM15 3a1 1 0 00-1 1v12a1 1 0 001 1h2a1 1 0 001-1V4a1 1 0 00-1-1h-2z",
          key: "library",
        },
      ],
    };
  },
};
</script>

<style></style>
