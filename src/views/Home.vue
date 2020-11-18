<template>
  <div class="home">
     <section id="FirstPage">
        <b-container>
            <b-card>
                    <h5>Untuk pemesanan<br>Silahkan masuk ke akun terlebih dahulu</h5>
                    <b-button variant="outline-primary">Masuk</b-button>
            </b-card>
        </b-container>
    </section>
    <section id="SecondPage">
        <div>
            <h1><br> <br>Paket Yang Tersedia</h1>
        </div>
        <b-container>
            <div class="row justify-content-center" style="margin-left: 35px;">
               <div>
                    <b-card
                      title="PAKET BRONZE"
                      img-src="./src/assets/bronze.jpg"
                      img-alt="Image"
                      img-top
                      tag="article"
                      style="max-width: 18rem;"
                      class="mb-2"
                    >
                      <b-card-text>
                        Paket ini bisa membersihkan secara bersih dan baik dengan menggunakan standar kebersihan 
                      </b-card-text>

                      <b-button href="#" variant="secondary">Pilih</b-button>
                    </b-card>
                  </div>
                  <div>
                    <b-card
                      title="PAKET SILVER"
                      img-src="assets/silver.png"
                      img-alt="Image"
                      img-top
                      tag="article"
                      style="max-width: 18rem;"
                      class="mb-2"
                    >
                      <b-card-text>
                        Paket ini bisa membersihkan secara bersih dan baik dengan menggunakan standar kebersihan 
                      </b-card-text>

                      <b-button href="#" variant="secondary">Pilih</b-button>
                    </b-card>
                  </div>
                  <div>
                    <b-card
                      title="PAKET GOLD"
                      img-src="../assets/Gold.jpg"
                      img-alt="Image"
                      img-top
                      tag="article"
                      style="max-width: 18rem;"
                      class="mb-2"
                    >
                      <b-card-text>
                        Paket ini bisa membersihkan secara bersih dan baik dengan menggunakan standar kebersihan 
                      </b-card-text>

                      <b-button href="#" variant="secondary">Pilih</b-button>
                    </b-card>
                  </div>
            </div>
        </b-container>
    </section>
    <section id="ThirdPage">
        <b-container>
            <h1 >Tentang Kami</h1>
            <p class="text-left">Sanitasi merupakan suatu bisnis yang bergerak dibidang jasa pembersihan ruangan di Yogyakarta.<br> Motto kami adalah “Bersih Bening” yang berarti kebersihan adalah tujuan utama kami.
                <br><br><br></p>
            <p class="text-left font-weight-bold"> <img src="image/phone-call.png" style="height: 25px; width: 25px;" /> 0877 9999 8888<br></p>
            <p class="text-left font-weight-bold"> <img src="image/envelope.png" style="height: 25px; width: 25px;" /> sanitasi@gmail.com<br></p>
        </b-container>
    </section>
 
  </div>

  
</template>
<style scoped>
#FirstPage .container {
    min-height: 100vh;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}
#FirstPage {
    background-image: url(../assets/halaman1.jpg);
    background-size: cover;
    height: 100%;
    width: 100%;
    background-position: top center;
    z-index: -4;
    opacity:
     .8;
}
html {
    scroll-behavior: smooth;
}

#SecondPage .h1 {
    margin-inline-start: -5px;
}
#SecondPage {
    background: whitesmoke;
    height: 600px;
    width: 100%;
    background-size: cover;
    z-index: -1;
    display: inline-block;
    opacity: .8;
}

#SecondPage .container {
    margin-top: 30px;
}

#SecondPage .card {
    background-color: #b4c7fb;
}



#ThirdPage {
    background-image: url(../assets/halaman3.png);
    background-size: cover;
    height: 700px;
    display: flex;
}

#ThirdPage .container {
    margin-block-start: 150px;
}

#ThirdPage .text-left {
    margin-inline-start: 600px;
}

#ThirdPage p {
    font-size: 1.1rem;
}
</style>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
