<template>
  <div>
    	<div class="container">
		<div class="card card-login mx-auto mt-5">
			<div class="card-header">Login</div>
			<div class="card-body">
				<form>
					<div class="form-group">
						<label for="email">Email</label>
						<input type="email" class="form-control" name="email" id="email" 
						placeholder="Digite seu Email">
					</div>
					<div class="form-group">
						<label for="senha">Senha</label>
						<input type="password" class="form-control" name="senha" id="senha" 
						placeholder="Digite sua Senha">
					</div>
					<div class="form-group">
						<div class="form-check">
							<label class="form-check-label">
								<input type="checkbox" class="form-check-input">
								Lembrar minha senha.
							</label>
						</div>
					</div>
					<button class="btn btn-primary btn-block">Entrar no Sistema</button>
					<div class="text-center">
						<nuxt-link to="/auth/register" class="d-block small mt-3"> Criar uma Conta</nuxt-link>
						<nuxt-link to="/auth/restore" class="d-block small"> Esqueceu a Senha?</nuxt-link>
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

            title:'Login',

			bodyAttrs: {
				class: 'bg-dark',
			},
    }
  },

  methods: {},
}
</script>

<style scoped></style>
