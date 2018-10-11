<template>
  <v-app dark>
    <v-toolbar flat>
      <v-toolbar-title>
        City:
      </v-toolbar-title>
      <v-toolbar-items>
        <v-btn flat>Hello</v-btn>
      </v-toolbar-items>      
    </v-toolbar>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data () {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [{
        icon: 'bubble_chart',
        title: 'Inspire'
      }],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
