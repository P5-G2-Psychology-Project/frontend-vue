<template>
  <nav>

    <img v-bind:src="require('./assets/we logo.png')" alt="" id="brand"/>
    <div>
      <form action="" id="form-login">
        <div class="form-group">
          <label id="name-label" for="name">e-mail</label>
          <input type="text" name="name" placeholder="Ingresa tu e-mail" required/>
       </div>
        <div class="form-group">
          <label id="name-label" for="name">password</label>
          <input type="password"  placeholder="Ingresa tu contraseña" required/>
       </div>
       <button type="submit">LogIn</button>
      </form>
    </div>
  </nav>


  <div class="main-component">
    <router-view
      v-on:completedLogIn="completedLogIn"
      v-on:completedSignUp="completedSignUp"
      v-on:logOut="logOut"
      v-on:completedTransaction="completedTransaction"
    >
    </router-view>
  </div>

</template>

<style>

  body {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
    padding: 0;
  }

  #brand {
    width: 100px;
    height: 100px;
    margin: 10px 26px;
  }

  nav {
    display: flex;
    position: fixed;
    top: 0;
    width: 100%;
    right: 0;
    justify-content: space-between;
    background-color: #f1f1f1;
  }

  #form-login{
    display: flex;
  }

  #form-login .form-group{
    display: flex;
    padding: 21px;
    flex-direction: column;
  }

  #form-login input {
    margin: 5px 0px;
    padding: 12px;
    border-radius: 18px;
    border: none;
  }

  #form-login button{
    width: 109px;
    height: 38px;
    margin-top: 54px;
    margin-right: 36px;
    border-radius: 15px;
    border: none;
    background-color: #a8baf0;
    color: white;
    font-size: 18px;
  }

  #form-login label{
    margin-left: 12px;
    font-size: 18px;
    font-weight: 100;
    margin-top: 9px;
    color: #6a6a6a;  
  }
  .main-component{
    width: 100%;
    margin: 0;
    padding: 0;
  }

</style>
