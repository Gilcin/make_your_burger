<template>
    <footer id="footer">
        <p>Mount Burger &copy; 2024</p>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>
    #footer {
        height: 200px;
        background-color: #222;
        border-top: 4px solid #111;
        color: #fcba03;
        display: flex;
        align-items: center;
        justify-content: center;
        margin-top: auto;
    }
    @media (max-width: 768px) {
  #footer {
    height: 80px;
  }
}

@media (max-width: 480px) {
  #footer {
    height: 60px;
  }
}
</style>