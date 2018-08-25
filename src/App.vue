<template>
  <v-app>

    <v-toolbar app :clipped-left="clipped">
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn flat>Link One</v-btn>
        <v-btn flat>Link Two</v-btn>
          <v-select
          :items="items"
          label="Outline style"
        ></v-select>
      </v-toolbar-items>
    </v-toolbar>

    <v-content>
      <Chef/>
    </v-content>

    <v-footer :fixed="fixed" app>
    </v-footer>

  </v-app>
</template>

<script>
import Chef from './components/Chef'

export default {
  name: 'App',
  components: {
    Chef
  },
  data () {
    return {
      items: ['Spanish', 'English'],
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
