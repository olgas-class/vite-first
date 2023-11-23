<script>
export default {
  data() {
    return {
      imageName: "milano.jpg",
    };
  },
  methods: {
    getImageUrl(imgName) {
        return new URL(`../assets/img/${imgName}`, import.meta.url).href;
    }
  }
};
</script>

<template>
  <!-- Metodo per immagine statica con path relativo -->
  <!-- <img src="../assets/img/milano.jpg" alt=""> -->

  <!-- Metodo per immagine statica con path assoluto -->
  <!-- <img src="/img/milano.jpg" alt=""> -->
  <!-- <div class="banner"></div> -->

  <!-- Metodo per immagini dinamici -->
  <img :src="getImageUrl(imageName)" alt="" />
</template>

<style scoped>
img {
  display: block;
  width: 80%;
  margin: 0 auto;
}

/* .banner {
    width: 80%;
    height: 400px;
    background-image: url(../assets/img/milano.jpg);
} */
</style>
