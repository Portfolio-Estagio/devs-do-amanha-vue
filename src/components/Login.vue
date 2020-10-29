<template>
  <div>
    <h2>Login</h2>
    <div class="hr hr-purple"></div>
    <form>
      <div class="form-group login-form">
        <label for="email">Email</label>
        <input class="form-control" type="email" required placeholder="Email" />
        <label for="pass">Senha</label>
        <input class="form-control" type="pass" required placeholder="Senha" />
        <br />
        <button class="btn btn-light">Entrar</button> ou
        <a href="#">Esqueci a senha</a>
      </div>
    </form>
  </div>
  <!-- <div>Teste</div> -->
</template>

<script>
export default {
  name: "Login",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
