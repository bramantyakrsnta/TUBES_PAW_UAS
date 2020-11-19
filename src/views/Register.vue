<template>
    <div class="register">
        <b-container style="margin-top: 10%;">
            <div id="registerbox">
                <h2>DAFTAR</h2>

                <hr>

                <div class="form-register">
                    <b-form @submit="onSubmit">
                        <b-row class="mt-4">
                            <b-col>
                                <b-form-group id="username-register" label-for="username-register">
                                    <b-form-input
                                        id="username"
                                        v-model="form.username"
                                        type="text"
                                        required
                                        placeholder="Username"
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                            <b-col>
                                <b-form-group id="password-register" label-for="password-register">
                                    <b-form-input
                                        id="password"
                                        v-model="form.password"
                                        type="password"
                                        required
                                        placeholder="Password"
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                        </b-row>
                        <b-row>
                            <b-col>
                                <b-form-group id="email-register" label-for="email-register">
                                    <b-form-input
                                        id="email"
                                        v-model="form.email"
                                        type="email"
                                        required
                                        placeholder="Email"
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                            <b-col>
                                <b-form-group id="notelp-register" label-for="notelp-register">
                                    <b-form-input
                                        id="notelp"
                                        v-model="form.notelp"
                                        type="number"
                                        required
                                        placeholder="Nomor Telepon"
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                        </b-row>
                        <b-row>
                            <b-col>
                                <b-form-group id="alamat-register" label-for="alamat-register">
                                    <b-form-input
                                        id="alamat"
                                        v-model="form.alamat"
                                        type="text"
                                        required
                                        placeholder="Alamat"
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                            <b-col>
                                <b-form-select v-model="selected" :options="jeniskelamin">
                                    <template #first>
                                        <b-form-select-option :value="null" disabled>-- Jenis Kelamin --</b-form-select-option>
                                    </template>
                                </b-form-select>
                            </b-col>
                        </b-row>
                        <b-row>
                            <b-col>
                                <div class="button mt-4" style="text-align: right;">
                                    <b-button type="reset" variant="danger">CANCEL</b-button>
                                </div>
                            </b-col>
                            <b-col>
                                <div class="button mt-4" style="text-align: left;">
                                    <b-button type="submit">SUBMIT</b-button>
                                </div>
                            </b-col>
                        </b-row>
                    </b-form>
                </div>

                <div id="login" class="mt-4" style="font-size: 12px; text-align: center; margin-bottom:-3%;">
                    <p>
                        sudah punya akun? 
                        <b-link href="/login">
                            klik disini
                        </b-link>
                    </p>
                </div>
            </div>
        </b-container>
    </div>
</template>

<script>
    export default {
        name: "Register",
        selected: null,
        data() {
            return {
                form: {
                    username: '',
                    password: '',
                    email: '',
                    notelp: null,
                    alamat: '',
                },
                jeniskelamin: [
                    { value: 'laki-laki', text: 'Laki-Laki' },
                    { value: 'perempuan', text: 'Perempuan' },
                ]
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

.register {
    text-align: center;
}

#registerbox {
    margin-left: 15%;
    width: 70%;
    padding: 3% 5% 5%;
    height: auto;
    background-color: #6c89d985;
    border-radius: 20px;
}

</style>