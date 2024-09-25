<script setup>

</script>

<template>
  <div id="app-container">
    <NavBar :logo="logo_src" :alt="app_name" />
    <main>
      <RouterView />
    </main>
    <Footer />
  </div>
</template>


<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    NavBar, 
    Footer
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Mount Burger"
    }
  }
}
</script>


<style>

#app-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* Garante que o app ocupe a altura total da viewport */
}


 * {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
 }

 .main-container{
  margin: 50px;
  min-height: 250px;
 }

 h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;

  @media (max-width: 768px) {
  .main-container {
    margin: 10px;
  }

  h1 {
    font-size: 24px;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 18px;
  }
}
 }
</style>
