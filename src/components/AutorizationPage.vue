<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="main">
    <img class = "logo" src="/src/assets/logo.png" alt="">
<div class="greetings">
    
    <div class="auth-meth">
      <h2>Методы аутентификации</h2>
 <details class="elem-auth">
        <summary >Мобильное приложение</summary>
        <a href="">
          <span>+ Добавить аккаунт</span>
        </a>
    </details>
    <details class="elem-auth">
        <summary >Telegram</summary>
        <a href="">
          <span>+ Добавить аккаунт</span>
        </a>
    </details>
    <details class="elem-auth">
        <summary >OTP-токены и приложения</summary>
        <a href="">
          <span>+ Добавить OTP</span>
        </a>
    </details>
    </div>
    <button class="end-setting">Завершить настройку</button>
  </div>

  </div>
 
    
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.logo{
    position: sticky;
    top: 0;
    color: white;
    padding: 15px;
    z-index: 100;
}

summary{
  margin-left: 15px;
}

.elem-auth{
width: 270px;
min-height: 50px;
background: #F0F4F7;
display: flex;
justify-content: center;
align-items: start;
flex-direction: column;
}

.greetings{
  background: #ffffff;
  display: flex;
  flex-direction: column;
  justify-content: start;
  align-items: center;
  text-align: center;
  height: 550px;
  width: 350px;
  box-shadow: 1px 2px 10px rgb(161, 159, 159);
  gap: 10px;
  border-radius: 20px;
}

.auth-meth{
  gap: 20px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 50px;
  
}

body{
   background: #316b92;
}
.main{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 100%;
  gap: 200px;
}

.end-setting{
  color: #ffffff;
  width: 250px;
  height: 40px;
  background: #579AD7;
  border-radius: 15px;
  border: none;
  margin-top: 50px;
}

@media (min-width: 1024px) {

}
</style>
