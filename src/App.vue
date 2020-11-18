<template>
  <div id="app">
    <b-nav class="navbar navbar-expand-sm fixed-top">
      <b-container class="container">
        <div>
          <img src="./assets/logo1.png" href="#" style="height: 65px; width: 65px;"/>
        </div>

        <b-navbar-brand href="#" class="toplogo" style="color: black; text-decoration: none; letter-spacing: 3px;"> SANITASI </b-navbar-brand>

        <b-collapse id="nav-collapse" is-nav>
          <b-nav class="ml-auto">
            <b-nav-item active id="beranda">BERANDA</b-nav-item>
            <b-nav-item id="paket">PAKET</b-nav-item>
            <b-nav-item id="tentangkami">TENTANG KAMI</b-nav-item>
            <b-button id="masuk" class="btn" href="/login" variant="outline-primary" aria-haspopup="true" aria-expanded="false"> MASUK </b-button>
          </b-nav>
        </b-collapse>
      </b-container>
    </b-nav>

    <router-view></router-view>

    <div class="footer">
      <b-container class="container" style="text-align: center;">
        <div id="box">
          <span></span>
        </div>
        <div>
          <img src="./assets/logo1.png"  style="height: 80px; width: 80px; text-align: center;"/>
        </div>
        <div class="mt-3">
          <span><h4>SANITASI</h4></span>
          <span><p>Copyright by Kelompok 4</p></span>
        </div>
      </b-container>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@600&display=swap');

#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  scroll-behavior: smooth;
}

.navbar {
  display: flex;
  justify-content: space-around;
  align-items: center;
  min-height: 8vh;
  background-color: #f4f4f4;
  border-bottom: 8px solid #6c89d9;
}

a.nav-link {
  color: black;
}

a.nav-link.active {
  color: black;
}

#masuk {
    color: #6c89d9;
    background-color: #f4f4f4;
}

.footer .container .toplogo {
  height: 100px;
  width: 100px;
}

.footer .container #box {
  text-align: center; 
  border-top: 8px solid #6c89d9; 
  margin-top: 80px;
  margin-bottom: 30px;
}

h4 {
  letter-spacing: 3px;
}

p {
  font-size: 10px;
}
</style>
