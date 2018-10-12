<template>
  <v-app dark>
    <v-toolbar flat>
      <v-toolbar-items>
        <v-select :items="cities" flat prepend-icon="map">
        </v-select>
      </v-toolbar-items>      
    </v-toolbar>
    hello
    <v-carousel :cycle="false">
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>
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
      cities: ['sacramento', 'sf bay area'],
      items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg'
        }]
    }
  }
}
</script>
