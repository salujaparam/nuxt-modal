
<template>
    <div class="header">
      <h3>Nuxt Modal</h3>
      <button @click="$emit('close-modal')">x</button>
    </div>
</template>
    
<style lang="css" scoped>
    .header {
        display: flex;
        justify-content: space-between;
    }
    h3{
        font-style: italic;
        padding: 10px 0px 0px 10px;
    }
    button {
        background: inherit;
        border: none;
        cursor: pointer;
        padding: 10px 10px 0px 0px;
        font-size: 1.2rem;
    }
</style>