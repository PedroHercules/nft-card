<template>
  <main>
    <Nft v-bind:nft="nft"/>
  </main>
</template>

<script>
  import Nft from '../components/Nft.vue';
  export default {
    data () {
      return {
        nft: {
          image: "../assets/img/image-equilibrium.png",
          title: "Equilibrium",
          description: "Our Equilibrium collection promotes balance and calm.",
          price: 0.041,
          expirationDays: 3,
          creator: "Jules Wyvern",
          photoCreator: "image-avatar.png"
        }
      }
    },
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
