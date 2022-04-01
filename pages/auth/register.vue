<template>
  <div>
    <div class="container">
      <div class="card card-register mx-auto mt-5">
        <div class="card-header">
          <span class="cor-purple">Criar uma Conta </span>
        </div>
        <div class="card-body">
          <form>
            <div class="form-group">
              <div class="form-row">
                <div class="col-md-6">
                  <span class="cor-purple">Criar uma Conta </span>
                  <label for="primeiroNome" class="cor-purple"
                    >Primeiro Nome</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="primeiroNome"
                    name="primeiroNome"
                    placeholder="Digite seu Primeiro Nome"
                  />
                </div>
                <div class="col-md-6">
                  <label
                    for="sobrenome"
                    class="cor-purple mt-3 mt-xl-0 mt-lg-0 mt-md-0"
                    >Sobrenome</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="sobrenome"
                    name="sobrenome"
                    placeholder="Digite seu Sobrenome"
                  />
                </div>
              </div>
            </div>
            <div class="form-group">
              <label for="email" class="cor-purple">Email</label>
              <input
                type="email"
                class="form-control"
                id="email"
                name="email"
                placeholder="Digite seu Email"
              />
            </div>
            <div class="form-group">
              <div class="form-row">
                <div class="col-md-6">
                  <label for="senha" class="cor-purple">Senha</label>
                  <input
                    type="password"
                    class="form-control"
                    id="senha"
                    name="senha"
                    placeholder="Digite uma Senha"
                  />
                </div>
                <div class="col-md-6">
                  <label
                    for="confirmaSenha"
                    class="cor-purple mt-3 mt-xl-0 mt-lg-0 mt-md-0"
                    >Confirmar Senha</label
                  >
                  <input
                    type="text"
                    class="form-control"
                    id="confirmaSenha"
                    name="confirmaSenha"
                    placeholder="Confirme sua Senha"
                  />
                </div>
              </div>
            </div>
            <button class="btn btn-pink text-white btn-block">
              Registrar-se
            </button>
            <div class="text-center">
              <nuxt-link
                to="/auth/restore"
                class="d-block small mt-3 cor-purple"
                >Esqueceu a senha?</nuxt-link
              >
              <nuxt-link to="/auth" class="d-block small cor-purple"
                >Página de Login</nuxt-link
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
  name: 'RegisterPage',

  layout: 'auth',

  data() {
    return {}
  },

  head() {
    return {
      title: 'Registrar',

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

input:checked {
  background-color: purple;
}
</style>
