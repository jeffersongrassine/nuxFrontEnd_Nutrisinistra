<template>
  <div>
    <div class="container">
      <div class="row mt-5 mr-4 justify-content-center">
        <nuxt-img
          src="logo-nova-Branca.png"
          sizes="sm:40vw md:40vw lg:200px"
          class="img-fluid -ml-2"
        />
      </div>
      <hr class="btn-pink" />
    </div>
    <div class="container text-center mt-5">
      <h3 v-if="error.statusCode === 404" class="text-white">
        Ops! Acho que aconteceu algo errado....
      </h3>
      <h3 v-else class="text-white">Ops! Acho que aconteceu algo errado....</h3>
      <NuxtLink to="/auth" class="cor-pink">Voltar ao site</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ErrorLayout',
  props: ['error'],
  layout: 'error',

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
  background-color: #f472b6;
}

input:checked {
  background-color: purple;
}
</style>
