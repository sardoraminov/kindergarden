<template>
  <div class="gallery-page">
    <div class="titles">
      <h1 class="title">Yutuqlar</h1>
      <p>(rasmlar va lavhalar)</p>
    </div>
    <div class="gallery">
      <div class="image" v-for="i in 48" :key="i">
        <img :src="require(`../assets/gallery/p${i}.jpg`)" alt="photo">
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 40px;
  padding: 0 20px;
}
.titles {
  text-align: center;
  margin-top: 50px;
}
.title {
  font-family: "Montserrat", sans-serif;
  font-size: 44px;
  font-weight: 900;
  background: linear-gradient(94.28deg, #ff595e 13.4%, #ffca3a 94.48%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

p {
  font-family: 'Manrope', sans-serif;
  font-size: 18px;  
}
</style>
