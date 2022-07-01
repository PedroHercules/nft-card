<template>
  <div id="card">
    <img src="../assets/img/image-equilibrium.jpg" alt="">
    <div id="info">
      <h2>Equilibrium #3429</h2>
      <p>Our Equilibrium collection promotes balance and calm.</p>
    </div>
  
    <div id="sub-info">
      <span>0.041 ETH</span>
      <span>3 days left</span>
    </div>

    <div id="created-by">
      <p>Creation of <span>Jules Wyvern</span></p>
    </div>
  </div>
</template>

<script setup>
  defineProps({
    nft: {
      type: Object,
      required: true
    }
  })
</script>

<style scoped>
  #card{
    display: flex;
    flex-direction: column;
    gap: 5px;
    padding: 15px 17px;
    width: 290px;
    height: 450px;
    background: hsl(216, 50%, 16%);
    border-radius: 1rem;
  }

  #card img {
    width: 100%;
    height: 220px;
    align-self: center;
    border-radius: .5rem;
  }
  
  h2{ 
    color: hsl(0, 0%, 100%);
    font-weight: 600;
  }

  p{
    color: hsl(215, 51%, 70%);
    font-size: 18px;
    font-weight: 400;
    margin-top: 0;
  }

  #sub-info{
    display: flex;
    justify-content: space-between;
    margin-top: 0;
    padding-bottom: 20px;
    border-bottom: 1px solid #fff;
  }

  span{
    color: hsl(178, 100%, 50%);
  }
  
</style>