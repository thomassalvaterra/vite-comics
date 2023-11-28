<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppFunzionalita from './components/AppFunzionalita.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppJumbo,
    AppFunzionalita,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <AppJumbo />
    <AppFunzionalita />
  </main>
  <AppFooter />
</template>

<style scoped></style>

