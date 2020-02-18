<template>
  <div>
    <h1>Modal using Nuxt.js</h1>
    <button class="btn" @click="openModal">Open Modal</button>
    <Modal class="modal" v-model="modalOpen" v-on:close-modal="closeModal"/>
  </div>
</template>

<script>
import Modal from '~/components/Modal'

export default {
  components: {
    Modal
  },
  data() {
    return {
          modalOpen: false
    };
  },
  methods: {
    openModal() {
            this.modalOpen = !this.modalOpen;
    },
    closeModal() {
      this.modalOpen = false
    }
  }
}
</script>

<style scoped>
  h1 {
    text-align: center;
  }
  button {
    position: absolute;
    left: 50%;
    top: 20%;
    transform: translate(-50%, -50%);
  }
  .modal {
    width: 25rem;
    position: absolute;
    left: 50%;
    top: 50%;
    min-height: 15rem;
    transform: translate(-50%, -50%);
    z-index: 1 !important;
  }
</style>
