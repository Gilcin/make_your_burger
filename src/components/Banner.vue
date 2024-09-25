<template>
    <div id="main-banner">
        <h1>Monte seu Burger</h1>
    </div>
</template>

<script>
    export default {
        name: "Banner"
    }

</script>

<style scoped>
    #main-banner {
    background-image: url('/img/burger.jpg');
    background-position: center;
    background-size: cover;
    height: 500px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    }

    #main-banner h1 {
        color: #fff;
        text-align: center;
        font-size: 60px;
        background-color: #b688094d;
        padding: 20px;
        border-radius: 5px;
    }

    @media (max-width: 1200px) {
  #main-banner {
    height: 400px;
  }
}

@media (max-width: 768px) {
  #main-banner {
    background-position: center;
    height: 400px;
  }

  #main-banner h1 {
    font-size: 40px;
    padding: 15px;
  }
}

@media (max-width: 480px) {
  #main-banner {
    background-position: center;
    height: 300px;
  }

  #main-banner h1 {
    font-size: 24px;
    padding: 10px;
  }
}

@media (min-width: 1600px) {
  #main-banner {
    height: 600px;
  }

  #main-banner h1 {
    font-size: 70px;
    padding: 25px;
  }
}

</style>