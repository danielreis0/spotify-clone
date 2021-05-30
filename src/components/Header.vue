<template>
  <div
    class=" flex flex-row items-center w-full h-16 bg-gray-900  sticky top-0 z-10 text-white   "
  >
    <div class="flex mx-8 items-center justify-between w-full ">
      <div class="flex justify-between ">
        <div
          class="flex justify-center items-center cursor-pointer bg-black rounded-full h-8 w-8 relative opacity-80"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 19l-7-7 7-7"
            />
          </svg>
        </div>
        <div
          class="hidden sm:inline-flex ml-4  justify-center items-center cursor-not-allowed bg-black rounded-full h-8 w-8 relative opacity-50"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 5l7 7-7 7"
            />
          </svg>
        </div>
      </div>
      <div class="flex">
        <div class="pr-8  hidden md:flex">
          <div
            class=" bg-black flex items-center cursor-pointer py-2 px-8 rounded-full bg-opacity-50 transform-gpu transition  hover:scale-105 border border-white border-opacity-50 hover:border-opacity-100 hover:bg-opacity-100"
          >
            <p class="text-xs font-semibold tracking-widest">
              FAÇA UPGRADE
            </p>
          </div>
        </div>

        <div class="flex">
          <div
            class="flex items-center relative cursor-pointer bg-black p-1  sm:pl-1 sm:pr-2 sm:py-2 rounded-full bg-opacity-70 hover:bg-gray-700"
          >
            <div
              class=" sm:absolute bg-gray-700 h-7 w-7  rounded-full flex justify-center items-center"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-4 w-4"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
                />
              </svg>
            </div>
            <p class="hidden sm:inline-flex pl-10 pr-6 text-sm font-bold ">
              danielreis003
            </p>
            <div class="hidden sm:flex relative justify-center items-center ">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-5 w-5 absolute mt-1 mr-4"
                viewBox="0 0 20 20"
                fill="currentColor"
              >
                <path
                  fill-rule="evenodd"
                  d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                  clip-rule="evenodd"
                />
              </svg>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
