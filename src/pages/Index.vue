<template>
  <q-page class="" padding>
    <!-- <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    > -->
    <input v-model="message" type="text" />
    <button @click="clearMessage">Clear</button>
    <h5>{{ message }}</h5>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      message: 'I love Vue.js'
    }
  },
  methods: {
    clearMessage() {
      this.message = ''
    }
  }
}
</script>
