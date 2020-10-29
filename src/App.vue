<template>
  <div style="padding: 10px; margin: 30px 0px;" class="row reg-area" id="app">
    <b-col class="p-4" v-if="modo">
      <h2>Sobre o site:</h2>
      <div class="hr hr-purple"></div>
      <p>
        Este é um site exclusivo para você, aluno, desenvolvedor e o que mais
        você quiser ser. Divirta-se e explore as diversas possibilidades no Devs
        do amanhã. Se você ainda não possui uma conta,
        <a @click="mode()" href="#">clique aqui</a>.
      </p>
    </b-col>

    <b-col class="p-4" v-if="modo">
      <Login />
    </b-col>
    
    <b-col class="p-4" v-else>
      <Register/> Já possui uma conta? <a @click="mode()" href="#">clique aqui</a> e entre.
    </b-col>
  </div>
</template>

<script>
import Login from "./components/Login.vue";
import Register from "./components/Register.vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";

export default {
  name: "App",
  components: {
    Login,
    Register,
  },
  data: () => {
    return{
      modo: true,
    }
  },
  methods:{
    mode(){
      this.modo = !this.modo;
    }
  }
};
</script>

<style>
@import url(../public/css/style.css);
</style>
