
<template>
  <div class="modal" v-show="value">
    <Header v-on:close-modal="$emit('close-modal')"/>
    <Body />
  </div>
</template>
    
<script>
import Header from './Header'
import Body from './Body'
  export default {
    name: 'Modal',
    components: {
      Body,
      Header
    },
    props: {
        value: {
          required: true
        }
    }
  };
</script>
    
    
<style lang="css" scoped>
  .modal {
    background-color: #DCDCDC;
  }
</style>