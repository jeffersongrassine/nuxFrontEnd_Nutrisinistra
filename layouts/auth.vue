<template>
  <div>
    <nuxt-link to="dashboard">
        <div class="container">
            <div class="row mt-5 mr-4 justify-content-center">
        <nuxt-img
          src="logo-nova-Branca.png"
          sizes="sm:40vw md:40vw lg:200px"
          class="img-fluid -ml-2"
        />
        <!-- <b-img center fluid width="200"  src="logo-nova-Branca.png" sizes="sm:50vw md:50vw lg:200px"></b-img> -->
      </div>
        </div>
      
    </nuxt-link>

    <nuxt />
  </div>
</template>

<script>
export default {
  name: 'AuthLayout',

  data() {
    return {}
  },

  methods: {},
}
</script>

<style scoped></style>
