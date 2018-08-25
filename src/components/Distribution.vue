<template>
    <v-select
      v-validate="'required'"
      :items="distributionList"
      v-model="distribution"
      label="Choose your Distribution"
      required
    ></v-select>
</template>

<script>
export default {
  name: 'Distribution',
  data () {
    return {
      'distributionList': [
        'LibreMesh',
        'LEDE',
        'OpenWRT'
      ],
      'distribution': ''
    }
  }
}
</script>
