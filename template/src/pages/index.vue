<template>
  <section class="container">
    <div>
      <hiu-logo/>
      <h1 class="title">
        hiu<b>Nuxt</b>
      </h1>
      <h2 class="subtitle">
        Nuxt.js project
      </h2>
      <!-- <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">Documentation</a>
        <a href="https://github.com/nuxt/nuxt.js" target="_blank" class="button--grey">GitHub</a>
      </div> -->
      <div class="links">
        <nuxt-link to="/list" class="button--grey">List</nuxt-link>
        <nuxt-link to="/backpages" class="button--grey">Backpages</nuxt-link>
        <nuxt-link to="/nuxt" class="button--green">Nuxt</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import hiuLogo from '~/components/hiu-logo.vue'

export default {
  // transition: '',
  components: {
    hiuLogo
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding-bottom: 10vh;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 100;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 22px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
