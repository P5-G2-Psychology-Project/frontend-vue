<template>
  <div class="home-component">
      <div>
        <img v-bind:src="require('../assets/illustration.jpg')" alt="" id="illustration"/>
      </div>
      <div class="signUpform">
        <h1>¿No tienes cuenta?</h1>
        <form action="">
          <div class="form-group">
            <label for="">Nombre</label>
            <input type="text" placeholder="Ingresa tu nombre"/>
          </div>
          <div class="form-group">
            <label for="">Correo</label>
            <input type="text" placeholder="example@example.com"/>
          </div>
          <div class="form-group">
            <label for="">Username</label>
            <input type="text" placeholder="Ingresa tu username"/>
          </div>
          <div class="form-group">
            <label for="" placeholder="Ingresa tu password">Password</label>
            <input type="text"/>
          </div>
          <button type="submit">SignUp</button>
        </form>
      </div>
  </div>
</template>

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
<style>

  .home-component{
    background: white;
    height: 657px;
    width: 100%;
    display: flex;
  }

  #illustration{
    width: 781px;
    margin-top: 99px;
  }

  .test {
    background: #d9ebfbbd;
    height: 657px;
    width: 100%;
  }
  .signUpform{
    margin-top: 150px;
    margin-left: 100px;
  }
  .signUpform h1{
    font-weight: 100;
    color: #424242;
    margin-bottom: 10px;
  }

  .signUpform input{
    margin: 5px 0px;
    padding: 12px;
    width: 129%;
    border-radius: 18px;
    border: 1px solid #a8baf0;
  }
  .signUpform .form-group{
    display: flex;
    flex-direction: column;
  }
  .signUpform button{
    width: 123px;
    height: 43px;
    margin-top: 10px;
    margin-right: 36px;
    border-radius: 21px;
    border: none;
    background-color: #a8baf0;
    color: white;
    font-size: 18px;
  }
  .signUpform label{
    margin-left: 12px;
    font-size: 18px;
    font-weight: 100;
    margin-top: 9px;
    color: #6a6a6a;    
  }
  
</style>