<template>
  <h4>{{title}}</h4>
  <div v-if="showModal">
  <Modal> 
  </Modal>
  </div>
  <button @click="toGle">klik</button>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  components: { Modal
    
  },
  name: 'App',
  data () {
    return {
      title: 'alo medo!',
      header: 'naglavu',
      text: 'mina skoci',
      showModal: false
    }
  },
  methods: {
    toGle () {
      this.showModal = !this.showModal
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
