<template>
  <main-page/>
</template>

<script>
import MainPage from './components/mainPage/main-page.vue'

export default {
  name: 'App',
  components: {
   MainPage
  }
}
</script>

<style>
li{
  list-style: none;
}
.container{
  max-width: 1230px;
  padding: 0 15px;
  margin: 0 auto;
}
</style>
