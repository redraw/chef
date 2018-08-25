<template>
  <v-container>
    <v-layout align-center justify-start column fill-height>
      <v-form v-model="valid">
        <distribution />
      </v-form>
    </v-layout>
  </v-container>
</template>

<script>
import Distribution from '@/components/Distribution'

export default {
  name: 'Chef',
  components: {
    Distribution
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
