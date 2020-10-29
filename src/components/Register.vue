<template>
  <div>
    <h2>Cadastro</h2>
    <div class="hr hr-purple"></div>
    <form>
      <div class="form-group login-form">
        <label for="email">Email</label>
        <input class="form-control" type="email" required placeholder="Email" />
        <label for="pass">Senha</label>
        <input class="form-control" type="pass" required placeholder="Senha" />
        <label for="confpass">Insira a senha novamente</label>
        <input class="form-control" type="pass" required placeholder="Confirmar senha" />
        <br/>
        <button class="btn btn-light">Registrar</button>
      </div>
    </form>
  </div>

  <!-- <div>Teste</div> -->
</template>

<script>
export default {
  name: "Register",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
