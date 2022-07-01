<template>
  <main>
    <Nft />
  </main>
</template>

<script>
  import Nft from '../components/Nft.vue';
  export default {
    components: {
      Nft
    }
  }
</script>

<style scoped>
  main {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
  }

</style>
