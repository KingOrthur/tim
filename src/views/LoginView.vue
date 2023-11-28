<template>
  <main>
    <div class="authorize">
      <div class="border-bott pb-2">
        ВХОД
      </div>
      <div class="line-input"></div>
      <form @submit="loginForm">
        <div class="mt-4 mb-3 email-container">
          <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Адрес эл.почты" v-model="email">
          <div class="errors" style="color: red">{{emailError}}</div>
        </div>
        <div class="mb-3 password-container">
          <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Пароль" v-model="password">
          <div class="errors" style="color: red">{{passwordError}}</div>
        </div>
        <button type="submit" class="btn btn-primary mt-4 mb-2 w-100">Войти</button>
<!--        <div class="authorize-password" >-->
<!--          <router-link :to="{name: 'home'}">Забыли пароль?</router-link>-->
<!--        </div>-->
        <div class="authorize-phone">
          <router-link :to="{name: 'register'}">Регистрация</router-link>
        </div>
      </form>
    </div>
  </main>
</template>

<script>
// import axios from "axios";
export default {
  name: "LoginView",
  data() {
    return {
      email: '',
      password: '',
      emailError: 'Заполните email',
      passwordError: 'Заполните пароль'
    }
  },
  methods: {
    loginForm(event){
      this.emailError = ''
      this.passwordError = ''

      if (this.email.trim() === ''){
        this.emailError = "Заполните email"
      }
      if (this.password.trim() === ''){
        this.passwordError = "Заполните пароль"
      }

      if (!this.emailError & !this.passwordError){
        const request = {
          email: this.email,
          password: this.password
        }
        // axios.post('http://localhost/api/user/login', request)
        //     .then((result) => {})
        //     .catch((error) => {
        //       alert(error.message)
        //     })
      }

      event.preventDefault()
    }
  }
}
</script>

<style scoped>

</style>