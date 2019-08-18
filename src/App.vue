<template>
  <div id="app" class="mt-16 text-gray-800 text-center">
    <img class="inline" src="./assets/logo.png">
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style lang="postcss">
  @import './assets/styles/main.css'
</style>
