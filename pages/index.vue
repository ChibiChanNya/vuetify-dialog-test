<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex>
      <v-icon>phone</v-icon>
    </v-flex>
    <v-flex>
      <v-icon>email</v-icon>
    </v-flex>
    <v-flex>
      <v-icon>place</v-icon>
    </v-flex>
    <v-flex>
      <v-icon>fab fa-facebook</v-icon>
    </v-flex>

    <v-btn big color="success" @click="showDialog">SHOW DIALOG</v-btn>
  </v-layout>
</template>

<script>

export default {
  components: {

  },

  methods: {
    showDialog(){
      this.$dialog.notify.success('TEST!',
        {
          position: 'top-middle',
          timeout: 5000
        })
    },
  },
}
</script>
