<template>
  <div class="hello">
    <h1 class="font-normal">{{ msg }}</h1>
    <h2 class="font-normal">Essential Links</h2>
    <InlineLinkList v-bind:links="essentialLinks"/>
    <h2 class="font-normal">Ecosystem</h2>
    <InlineLinkList v-bind:links="ecosystemLinks"/>
  </div>
</template>

<script>
import InlineLinkList from './InlineLinkList'

export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      essentialLinks: [
        {
          url: 'https://vuejs.org',
          text: 'Core Docs'
        },
        {
          url: 'https://forum.vuejs.org',
          text: 'Forum'
        },
        {
          url: 'https://chat.vuejs.org',
          text: 'Community Chat'
        },
        {
          url: 'https://twitter.com/vuejs',
          text: 'Twitter'
        },
        {
          url: 'http://vuejs-templates.github.io/webpack/',
          text: 'Docs for This Template'
        }
      ],
      ecosystemLinks: [
        {
          url: 'http://router.vuejs.org/',
          text: 'vue-router'
        },
        {
          url: 'http://vuex.vuejs.org/',
          text: 'vuex'
        },
        {
          url: 'http://vue-loader.vuejs.org/',
          text: 'vue-loader'
        },
        {
          url: 'https://github.com/vuejs/awesome-vue',
          text: 'awesome-vue'
        }
      ]
    }
  },
  components: {
	  InlineLinkList
  }
}
</script>
