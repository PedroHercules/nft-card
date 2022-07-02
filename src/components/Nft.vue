<template>
  <div id="card">
    <div id="image-nft">
      <img src="../assets/img/image-equilibrium.jpg" alt="sss">
      <div id="hover-nft">
        <img src="./icons/icon-view.svg" alt="view" />
      </div>
    </div>
    
    <div id="info">
      <h2> <a href="#">Equilibrium &#35;3429</a> </h2>
      <p>Our Equilibrium collection promotes balance and calm.</p>
    </div>
  
    <div id="sub-info">
      <span>
        <img id="icon-eth" src="./icons/icon-ethereum.svg" alt="eth" /> 
        0.041 ETH 
      </span>
      <span>
        <img id="icon-clock" src="./icons/icon-clock.svg" alt="clock" />
        3 days left
      </span>
    </div>

    <div id="created-by">
      <img src="../assets/img/image-avatar.png" alt="avatar" />
      <span>Creation of <a href="#">Jules Wyvern</a></span>
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
    height: 500px;
    background: hsl(216, 50%, 16%);
    border-radius: 1rem;
  }

  #image-nft {
    width: 100%;
    height: 250px;
    align-self: center;
    border-radius: .5rem;
    position: relative;
    
  }

  #image-nft img{
    width: 100%;
    height: 250px;
    border-radius: .5rem;
  }

  #hover-nft {
    display: none;
    width: 100%;
    height: 250px;
    background: rgba(0, 255, 247, .3);
    justify-content: center;
    align-items: center;
    top: 0;
    position: absolute;
    border-radius: .5rem;
  }

  #hover-nft img{
    width: 30px;
    height: 30px;
  }

  #image-nft img:hover + #hover-nft{
    display: flex;
    
  }

  #image-nft:hover{
    cursor: pointer;
  }

  #image-nft img:hover{
    
    cursor: pointer;
  }

  #card img:hover{
    background: 000;
    z-index: 9999;
    cursor: pointer;
  }
  

  h2 a{
    text-decoration: none;
    color: hsl(0, 0%, 100%);
    font-weight: 600;
    transition: .3s;
  }

  h2 a:hover{
    color: hsl(178, 100%, 50%);
  }

  p{
    color: hsl(215, 51%, 70%);
    font-size: 18px;
    font-weight: 400;
    margin-top: 0;
  }

  #sub-info{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 0;
    padding-bottom: 20px;
    border-bottom: 1px solid #fff;
  }

  span{
    color: hsl(178, 100%, 50%);
  }

  #sub-info span{
    display: flex;
    gap: 5px;
  }

  #sub-info #icon-eth{
    width: 10px;
    height: 20px;
  }

  #sub-info #icon-clock{
    width: 20px;
    height: 20px;
  }

  #created-by {
    display: flex;
    align-items: center;
    gap: 5px;
    padding: 20px 0;
  }
  
  #created-by img{
    width: 30px;
    height: 30px;
    border: 1px solid #fff;
    border-radius: 100%;
  }

  #created-by span{
    color: hsl(215, 51%, 70%);
  }

  #created-by span a{
    color: hsl(0, 0%, 100%);
    text-decoration: none;
    transition: .3s;
  }

  #created-by span a:hover{
    color: hsl(178, 100%, 50%);
  }
</style>