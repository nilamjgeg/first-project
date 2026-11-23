<script setup>
import { ref, reactive, computed, watch } from "vue";

// const data = {
//   link: "www.facebook.com",
//   name: "facebook",
//   imgUrl:
//     "https://www.google.com/imgres?q=sofia%20the%20first&imgurl=https%3A%2F%2Fwww.hollywoodreporter.com%2Fwp-content%2Fuploads%2F2012%2F11%2Fsofia_the_first_characters_a_p.jpg%3Fw%3D1440%26h%3D810%26crop%3D1&imgrefurl=https%3A%2F%2Fwww.hollywoodreporter.com%2Fnews%2Fgeneral-news%2Fdisneys-sofia-first-tv-series-394349%2F&docid=aHna78tbPlhGlM&tbnid=wlcGmKtobbcDEM&vet=12ahUKEwjk2d7A19yXAxUQ4zgGHRJcK5UQnPAOegQIPRAA..i&w=349&h=466&hcb=2&ved=2ahUKEwjk2d7A19yXAxUQ4zgGHRJcK5UQnPAOegQIPRAA",
//   altText: "Rapunzel",
//   value: "jus kiding",
// };

let produk = [
  { nama: "Bakpao", bentuk: "Bulat", rasa: "coklat" },
  { nama: "Donat", bentuk: "Lonjong", rasa: "oreo" },
  { nama: "cheesecake", bentuk: "Segitiga", rasa: "blueberry" },
];
</script>

<template>
  <!-- <a :href="data.link">{{ data.name }}</a>
  <img :src="data.imgUrl" :alt="data.altText" />
  <input type="text" :value="data.value" /> -->

  <div v-for="(item, index) in produk" :key="index">
    <h2>{{ item.nama }}</h2>
    <p>{{ item.rasa }}</p>
    <p>{{ item.bentuk }}</p>
  </div>
</template>

<style scoped></style>
