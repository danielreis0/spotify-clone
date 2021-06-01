<template>
  <div id="app" class="bg-main flex ">
    <side-bar />
    <div class="w-full">
      <Header />
      <home-cards :data="homeCardsData" />
      <section-cards :data="sectionCardsData" />
      <section-cards :data="sectionCardsData2" />
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
      sectionCardsData: {
        title: "Programas para conhecer",
        subtitle: "Podcasts que achamos que você vai adorar.",
        cards: [
          {
            id: 1,
            title: "Canções de TFM",
            author: "Canções de TFM",
            img:
              "https://i.scdn.co/image/2176e6517c0d86bc58504ddd84772a2f98fb044c",
          },
          {
            id: 2,
            title: "Harry Potter E a Pedra Filosofal",
            author: "Harry Potter E a Pedra Filosofal",
            img:
              "https://i.scdn.co/image/902bedd6cc3cc465e23174ac33c618177fa262da",
          },
          {
            id: 3,
            title: "Histórias de Runeterra",
            author: "Consta",
            img:
              "https://i.scdn.co/image/5032d0f947f7882598c1eb35d84b95b7eb5360b4",
          },
          {
            id: 4,
            title: "Dr. Pimpolho",
            author: "Felipe Xavier",
            img:
              "https://i.scdn.co/image/6aa84050c63117d9c1c728429ee89a47fb657240",
          },
          {
            id: 5,
            title: "Áudios Vazados",
            author: "VoxMojo",
            img:
              "https://i.scdn.co/image/1153d11c78e8b04ec1bbf3bb7d5505876a20b4cd",
          },
        ],
      },
      sectionCardsData2: {
        title: "Suas Músicas Estão com saudade",
        subtitle: "",
        cards: [
          {
            id: 1,
            title: "Sandy e Junior",
            img:
              "https://i.scdn.co/image/7e43bb526316a72e8a922d44e29e70c4e417d0e6",
            type: "Artista",
            playable: true,
          },
          {
            id: 2,
            title: "Grupo Menos É Mais",
            type: "Artista",
            img:
              "https://i.scdn.co/image/0c95ca56a84f8708643647e7d333e99fe3b8d8f0",
            playable: true,
          },
          {
            id: 3,
            title: "Good Times (Flash Back)",
            user: "Marcos Paulo",
            img:
              "https://i.scdn.co/image/ab67706c0000da844d37a1f743259a1e0ef9143e",
            playable: true,
          },
          {
            id: 4,
            title: "Mac Miller",
            type: "Artista",
            img:
              "https://i.scdn.co/image/ed63d93ec5348edc9cdf85c97179bbc78cd57292",
            playable: true,
          },
          {
            id: 5,
            title: "The Jackson 5",
            type: "Artista",
            img:
              "https://i.scdn.co/image/19f768d93f6c80f7d4ca5b906e1c0376a3704389",
            playable: true,
          },
        ],
      },
    };
  },
};
</script>

<style>
* {
  font-family: "Heebo", sans-serif;
}
</style>
