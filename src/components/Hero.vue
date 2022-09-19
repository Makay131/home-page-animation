<template>
  <div class="hero">
    <nav class="navbar">
      <p class="logo">PW&nbsp;House</p>
      <button class="btn">Subscribe</button>
    </nav>
    <div class="content">
      <small class="small">Welcome to the</small>
      <h1>World's Creative <br>Pizzeria</h1>
      <button class="btn">Take a Tour</button>
      <div class="icons">
        <div class="icon__container"><ion-icon name="logo-instagram"></ion-icon></div>
        <div class="icon__container"><ion-icon name="logo-twitter"></ion-icon></div>
        <div class="icon__container"><ion-icon name="logo-facebook"></ion-icon></div>
        <div class="icon__container"><ion-icon name="logo-whatsapp"></ion-icon></div>
    </div>
    <div class="bubbles">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
    <img src="../assets/bubble.png" alt="bubble">
  </div>
  </div>

  
  </div>
</template>

<script>
export default {
  name: 'Hero',
}
</script>

<style scoped>
  .hero {
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(to top, rgba(245, 246, 252, 0.08), rgba(75, 12, 59, 0.73)),
                      url(../assets/jonathan-formento-Agukhm5v0lA-unsplash.jpg);

    background-size: cover;
    background-position: center;
    overflow: hidden;
    position: relative;
  }
  .navbar {
    width: 80%;
    height: 20%;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .content {
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-direction: column;
    height: calc(100% - 20%);
    z-index: 9;
    text-align: center;

    color: #e9c6f1;
    
  }
  .logo {
    font-size: 1.6rem;
    font-weight: 600;
    letter-spacing: .8;
    color: #e7e8ee;
    cursor: pointer;
  }
  .btn {
    background: transparent;
    border: 1px solid #e7e8ee;
    outline: none;
    padding: 10px 25px;
    cursor: pointer;
    border-radius: 15px;
    color: #e7e8ee;
    font-size: 1.1rem;
    font-weight: 300;

    transition: all .4s ease;
  }
  .btn:hover {
    border: 1px solid transparent;
    color: #e7e8ee;
    transform: scale(1.1);
  }
  .small {
    font-size: 1rem;
    font-weight: 600;
    text-transform: uppercase;
    margin-bottom: 10px;
  }

  .icons {
    display: flex;
    gap: 10px;
  }

  .icon__container {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: linear-gradient(#e9c6f125, #320353f3);
    cursor: pointer;

    position: relative;
    transition: all .4s ease;
  }

  .icon__container:hover {
    transform: translateY(-2px);
    scale: 1.05;
  }

  ion-icon {
    width: 20px;
    height: 20px;
    color: #e9c6f1;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .bubbles img{
    width: 50px;
    filter: hue-rotate(100deg);
    animation: bubble 7s linear infinite;
  }

  .bubbles {
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;

    position: absolute;
    bottom: -60px;
  }

  @keyframes bubble {
    0% {
      transform: translateY(0);
      opacity: 0;
    }
    50% {
      
      opacity: 1;
    }
    70% {
      
      opacity: 1;
    }
    100% {
      transform: translateY(-80vh);
      opacity: 0;
    }
  }

  .bubbles img:nth-child(1) {
    animation-delay: 2s;
    width: 25px;
  }
  .bubbles img:nth-child(2) {
    animation-delay: 1s;
  }
  .bubbles img:nth-child(3) {
    animation-delay: 3s;
    width: 25px;
  }
  .bubbles img:nth-child(4) {
    animation-delay: 4.5s;
  }
  .bubbles img:nth-child(5) {
    animation-delay: 3s;
  }
  .bubbles img:nth-child(6) {
    animation-delay: 6s;
    width: 20px;
  }
  .bubbles img:nth-child(7) {
    animation-delay: 7s;
    width: 35px;
  }
</style>
