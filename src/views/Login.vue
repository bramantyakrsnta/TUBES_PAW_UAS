<template>
  <div class="login">
    <b-container style="margin-top: 10%;">
      <div id="loginbox">
        <h2 style="margin-top: -30px;">MASUK</h2>

        <hr>

        <div class="form-login">
          <b-form @submit="onSubmit">
            <b-form-group id="username-input" label-for="username-input">
              <b-form-input
                id="username"
                v-model="form.username"
                type="text"
                required
                placeholder="Username"
              ></b-form-input>
            </b-form-group>

            <b-form-group id="password-input" label-for="password-input">
              <b-form-input
                id="password"
                v-model="form.password"
                type="password"
                required
                placeholder="Password"
              ></b-form-input>
            </b-form-group>

            <div id="register" class="ml-2" style="font-size: 12px; text-align: left;">
              <p>
                belum punya akun? 
                  <b-link href="#">
                    klik disini
                  </b-link>
                </p>
            </div>

            <div class="button mt-4" style="margin-bottom: -30px; text-align: right;">
              <b-button type="submit">SUBMIT</b-button>
            </div>
          </b-form>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
  export default {
    name: "Login",
    data() {
      return {
        form: {
          username: '',
          password: '',
        },
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        // alert(JSON.stringify(this.form))
        alert("Login Berhasil!")
      },
    }
  }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@600&display=swap');

* {
  font-family: 'Montserrat', sans-serif;
}

.login {
  text-align: center;
}

#loginbox {
  margin-left: 30%;
  width: 40%;
  height: auto;
  padding: 6%;
  height: auto;
  background-color: #6c89d985;
  border-radius: 20px;
}

</style>