<template>
  <div>
    <div class="container">
      <div class="card card-login mx-auto mt-5">
        <div class="card-header">Recuperar Senha</div>
        <div class="card-body">
          <div class="text-center mt-4 mb-5">
            <h4>Esqueceu sua senha?</h4>
            <p>
              Digite seu email e nós lhe enviaremos intruções sobre como
              redefinir sua senha.
            </p>
          </div>
          <form>
            <div class="form-group">
              <label for="email">Email</label>
              <input
                type="email"
                class="form-control"
                name="email"
                id="email"
                placeholder="Digite seu Email"
              />
            </div>
            <button class="btn btn-primary btn-block">Recuperar Senha</button>
            <div class="text-center">
              <nuxt-link to="/auth/register" class="d-block small mt-3">Criar uma Conta</nuxt-link>
              <nuxt-link to="/auth" class="d-block small">Página de Login</nuxt-link>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegisterPage',

  data() {
    return {}
  },

  head() {
    return {
      title: 'Recuperar Senha',

      bodyAttrs: {
        class: 'bg-dark',
      },
    }
  },

  methods: {},
}
</script>

<style scoped></style>
