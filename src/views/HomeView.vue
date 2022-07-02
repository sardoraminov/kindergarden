<template>
  <div class="home-page">
    <div class="page-titles">
      <h1 class="title">
        Yuldasheva Feruzaxon <br />
        <b>Azamat qizi</b>
      </h1>
      <p class="desc">
        UrDU Maktabgacha ta’lim fakulteti 3-kurs talabasi <br />
        Tajribasi 1 yil 3 oy
      </p>
      <p class="desc">
        Xorazm viloyati Gurlan tumani 8-son "Quyoshcha" maktabgacha <br />
        ta'lim tashkilotida tarbiyachi
      </p>
    </div>
    <router-link to="/gallery" class="page-link">
      <span class="text">Yutuqlar</span></router-link
    >
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped>
.page-link {
  text-decoration: none;
  padding: 15px 30px;
  border-radius: 99px;
  transition: all 0.7s ease;
  position: relative;
  background: linear-gradient(94.28deg, #ff595e 13.4%, #ffca3a 94.48%);
  background-size: 100% 100%;
}

.page-link:hover {
  background-size: 400% 400%;
}

.page-link .text {
  color: #fff;
  font-family: "Montserrat", sans-serif;
  font-size: 18px;
  text-transform: uppercase;
  font-weight: 700;
}
.home-page {
  height: 100vh;
  background: url(../assets/bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  text-align: center;
}

.title {
  font-family: "Manrope", sans-serif;
  font-family: "Montserrat", sans-serif;
  background: linear-gradient(94.28deg, #ff595e 13.4%, #ffca3a 94.48%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  padding-top: 100px;
  font-size: 44px;
}

b {
  font-family: "Montserrat", sans-serif !important;
  font-size: 68px;
  font-weight: 900;
  line-height: 36px;
}

.desc {
  font-family: "Manrope", sans-serif;
  font-weight: 600;
  margin: 20px;
  font-size: 24px;
  color: #333;
}

.desc:first-child {
  margin-top: 45px;
}

.desc:last-child {
  margin-bottom: 50px;
}

@media (max-width: 952px) {
  .home-page {
    background-position: left left;
    background-attachment: fixed;
  }
}

@media (max-width: 639px) {
  .home-page {
    background: url(../assets/bg-resp.jpg);
    background-size: cover;
    background-repeat: no-repeat;
  }

  .title {
    font-size: 28px;
  }

  b {
    font-size: 44px;
  }

  .desc {
    font-size: 16px;
  }

  .page-titles {
    padding: 0 10px;
  } 
}

</style>
