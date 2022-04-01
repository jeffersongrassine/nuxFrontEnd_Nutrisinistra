<template>
	<div>
		 <div class="container">
		<div class="card card-register mx-auto mt-5">
			<div class="card-header">Criar uma Conta</div>
			<div class="card-body">
				
				<form>
					<div class="form-group">
						<div class="form-row">
							<div class="col-md-6">
								<label for="primeiroNome">Primeiro Nome</label>
								<input type="text" class="form-control" id="primeiroNome" name="primeiroNome"
								placeholder="Digite seu Primeiro Nome">
							</div>
							<div class="col-md-6">
								<label for="sobrenome">Sobrenome</label>
								<input type="text" class="form-control" id="sobrenome" name="sobrenome"
								placeholder="Digite seu Sobrenome">
							</div>					
						</div>
					</div>
					<div class="form-group">
						<label for="email">Email</label>
						<input type="email" class="form-control" id="email" name="email"
						placeholder="Digite seu Email">
					</div>
					<div class="form-group">
						<div class="form-row">
							<div class="col-md-6">
								<label for="senha">Senha</label>
								<input type="password" class="form-control" id="senha" name="senha"
								placeholder="Digite uma Senha">
							</div>
							<div class="col-md-6">
								<label for="confirmaSenha">Confirmar Senha</label>
								<input type="text" class="form-control" id="confirmaSenha" name="confirmaSenha"
								placeholder="Confirme sua Senha">
							</div>					
						</div>
					</div>
					<button class="btn btn-primary btn-block">Registrar-se</button>
					<div class="text-center">
						<nuxt-link to="/restore" class="d-block small mt-3">Esqueceu a senha?</nuxt-link>
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
			return {
				 
			};
		},

		 head() {
        return {

            title:'Registrar',

			bodyAttrs: {
				class: 'bg-dark',
			},
    }
  },

		methods: {}
	};
</script>

<style scoped>
	 
</style>



