<script>
  export default {
    data() {
      return {
        currentBackgroundImage: ''
      };
    },
    methods: {
      changeBackground(image) {
        this.currentBackgroundImage = `url(${image})`; 
      },
      resetBackground() {
        this.currentBackgroundImage = ''; 
      }
    }
  };
</script>

<template>
  <div 
    class="about" 
    :style="{ backgroundColor: defaultBackgroundColor, backgroundImage: currentBackgroundImage }"
  >
    <h1 class="heading">About Me</h1>
    <div class="container">
      <p>
        Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
        Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
        Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
        Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit.
      </p>
      <div class="images">
        <img 
          src="../assets/images/gamesConsole.jfif" 
          alt="image1"
          @mouseover="changeBackground('/src/assets/images/gamesConsole.jfif')" 
          @mouseleave="resetBackground"
        >
        <img 
          src="../assets/images/coffee.jfif" 
          alt="image2"
          @mouseover="changeBackground('/src/assets/images/coffee.jfif')" 
          @mouseleave="resetBackground"
        >
        <img 
          src="../assets/images/dogs.jfif" 
          alt="image3"
          @mouseover="changeBackground('/src/assets/images/dogs.jfif')" 
          @mouseleave="resetBackground"
        >
      </div>
    </div>
  </div>
</template>

<style scoped>
  .images {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }

  .images img:nth-child(2) {
    margin-top: 150px;
  }

  .images img:nth-child(3) {
    margin-top: -150px;
  }

  .images img:hover {
    transform: scale(1.1);
    box-shadow: 0px 4px 20px rgba(255, 255, 255, 0.5);
  }

  img {
    width: 300px;
    height: 250px;
    object-fit: cover;
    
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    margin-bottom: 10px;
  }

  .container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }

  .about {
    display: flex;
    flex-direction: column;
    gap: 16px;
    transition: background-image 0.5s ease-in-out;
    background-size: cover;
    background-position: center;
    min-height: 100vh;
    padding: 20px;
  }

  @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  }
</style>



