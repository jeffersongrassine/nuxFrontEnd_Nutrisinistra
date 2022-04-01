<template>
  <div>
    <div class="container">
      <div class="card card-login mx-auto mt-5">
        <div class="card-header">
          <span class="cor-purple">Login</span>
        </div>
        <div class="card-body">
          <form>
            <div class="form-group">
              <label for="email" class="cor-purple">Email</label>
              <input
                type="email"
                class="form-control"
                name="email"
                id="email"
                placeholder="Digite seu Email"
              />
            </div>
            <div class="form-group">
              <label for="senha" class="cor-purple">Senha</label>
              <input
                type="password"
                class="form-control"
                name="senha"
                id="senha"
                placeholder="Digite sua Senha"
              />
            </div>
            <div class="form-group">
              <div class="form-check">
                <label class="form-check-label">
                  <input type="checkbox" class="form-check-input cor-puple" />
                  <span class="cor-purple">Lembrar minha senha.</span>
                </label>
              </div>
            </div>
            <button class="btn btn-pink btn-purple:hover text-white btn-block">
              Entrar no Sistema
            </button>
            <div class="text-center">
              <nuxt-link
                to="/auth/register"
                class="d-block small mt-3 cor-purple"
              >
                Criar uma Conta</nuxt-link
              >
              <nuxt-link to="/auth/restore" class="d-block small cor-purple">
                Esqueceu a Senha?</nuxt-link
              >
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AuthPage',

  layout: 'auth',

  data() {
    return {}
  },

  head() {
    return {
      title: 'Login',

      bodyAttrs: {
        class: 'bg-dark',
      },
    }
  },

  methods: {},
}
</script>

<style scoped>
.btn-pink {
  background-color: #be185d;
}

.btn-pink:hover {
  background-color: #e83e8c;
}

.cor-pink {
  color: #e83e8c;
}
cor-pink:hover {
  color: #f472b6;
}

.cor-purple {
  color: purple;
}

.bg-pink-400 {
  background-color: #f472b6 ;
}

input:checked {
  background-color: purple;
}
</style>
