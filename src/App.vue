<template>
  <div id="app" class="bg-main flex ">
    <side-bar />
    <div class="w-full">
      <Header />
      <home-cards :data="homeCardsData" />

      <section-cards />
    </div>
  </div>
</template>

<script>
import "tailwindcss/tailwind.css";
import SideBar from "@/components/SideBar";
import Header from "@/components/Header";
import HomeCards from "@/components/HomeCards";
import SectionCards from "@/components/SectionCards";

export default {
  name: "App",
  components: {
    SideBar,
    Header,
    HomeCards,
    SectionCards,
  },
  data() {
    return {
      homeCardsData: [
        {
          id: 1,
          title: "Mac Miller",
          img:
            "https://i.scdn.co/image/ed63d93ec5348edc9cdf85c97179bbc78cd57292",
        },
        {
          id: 2,
          title: "The Weeknd",
          img:
            "https://i.scdn.co/image/37376dba0623c33923eae9d234e5e199b76d227f",
        },
        {
          id: 3,
          title: "Exaltasamba",
          img:
            "https://i.scdn.co/image/ab67616d0000b27376cb9dbfee72b93bc8d8938b",
        },
        {
          id: 4,
          title: "Good Times (Flash Back)",
          img:
            "https://i.scdn.co/image/ab67706c0000bebb4d37a1f743259a1e0ef9143e",
        },
        {
          id: 5,
          title: "Racionais MC",
          img:
            "https://i.scdn.co/image/0e9f58b86b301af364cc4c130a4b19a86f75af73",
        },
        {
          id: 6,
          title: "Sandy e Junior",
          img:
            "https://i.scdn.co/image/7e43bb526316a72e8a922d44e29e70c4e417d0e6",
        },
      ],
    };
  },
};
</script>

<style>
* {
  font-family: "Heebo", sans-serif;
}
</style>
