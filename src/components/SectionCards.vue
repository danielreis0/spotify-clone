<template>
  <div class="flex flex-col my-10 ">
    <div class="text-white w-full px-4 md:px-8  flex flex-col ">
      <div class="flex ">
        <h1
          class="text-xl    font-semibold cursor-pointer hover:underline select-none  "
        >
          Programas para conhecer
        </h1>
      </div>
      <div class=" flex justify-between ">
        <p class="text-sm  text-gray-400 ">
          Podcast que achamos que você vai adorar.
        </p>
        <p
          class="hidden sm:flex text-sm font-medium  hover:underline cursor-pointer text-gray-400 "
        >
          VER TUDO
        </p>
      </div>
    </div>

    <div class="px-4 md:px-8 mt-3 ">
      <div class="grid grid-cols-footer  gap-6">
        <div
          v-for="n in 5"
          :key="n"
          class="flex flex-col transform-gpu hover:-translate-y-1 justify-center items-center bg-gray-800 text-white rounded-md select-none cursor-pointer transition ease-in-out bg-opacity-30 hover:bg-opacity-80"
        >
          <div class=" h-auto w-full p-4 flex justify-center items-center ">
            <img
              class="w-40 h-auto  bg-green-900  rounded-xl shadow-lg"
              src="https://i.scdn.co/image/1153d11c78e8b04ec1bbf3bb7d5505876a20b4cd"
              alt=""
            />
          </div>

          <div class="  px-4 w-full pb-6">
            <h3 class="text-white text-base font-medium">Áudios Vazados</h3>
            <p class="text-gray-400 text-sm">VoxMojo</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
