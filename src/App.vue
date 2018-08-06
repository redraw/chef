<template>
  <v-app>

    <v-toolbar
      app
      :clipped-left="clipped"
    >
      <v-toolbar-title v-text="title"></v-toolbar-title>
    </v-toolbar>

    <v-content>
      <ImageBuilder/>
    </v-content>

    <v-footer :fixed="fixed" app>
      <span>&copy; 2017</span>
    </v-footer>

  </v-app>
</template>

<script>
import ImageBuilder from './components/ImageBuilder'

export default {
  name: 'App',
  components: {
    ImageBuilder
  },
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [{
        icon: 'bubble_chart',
        title: 'Inspire'
      }],
      miniVariant: false,
      right: false,
      rightDrawer: false,
      title: 'Chef ImageBuilder 0.11'
    }
  }
}
</script>
