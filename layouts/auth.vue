<template>
  <div>
    <div class="img-fluid img align-items-lg-center">
      <nuxt-link to="dashboard">
        <nuxt-img src="logo-nova-Branca.png" sizes="sm:50vw md:50vw lg:200px"  />
      </nuxt-link>
    </div>

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
