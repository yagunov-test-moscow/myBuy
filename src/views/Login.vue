<template>
  <div class="row">
    <div class="col s12 m6">
  <form class="card auth-card" 
  style="
  border-radius: 10px;
  padding: 10px 10px 40px;">
    <div class="card-content">
      <span class="card-title" style="text-align: center;">MyBuy</span>
      <span class="card-title" style="text-align: center; margin-top: 30px;">Вход</span>
      <div class="input-field">
        <input
            id="email"
            type="text"
        >
        <label for="email">Email</label>
        <small 
          class="helper-text invalid"
        >Поле email не должно быть пустым</small>
        <small 
          class="helper-text invalid"
        >Введите корректный email</small>
      </div>
      <div class="input-field">
        <input
            id="password"
            type="password"
        >
        <label for="password">Пароль</label>
        <small 
          class="helper-text invalid"
        >Введите пароль</small>
        <small 
          class="helper-text invalid"
        >Пароль должен быть больше  символов. Сейчас он  </small>
      </div>
    </div>
    <div class="card-action" style="padding: 20px;">
          <button
              class="btn waves-effect light-blue darken-2 right" style="text-transform: none;"
              type="submit"
          > Войти
          </button>

      <p class="left light-blue-text text-darken-2">
        <router-link class="light-blue-text text-darken-2 left" style="text-transform: none;" to="/register">Создать аккаунт</router-link>
      </p>
    </div>
  </form>
   </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.card .card-action {
  padding: 20px;
}
</style>