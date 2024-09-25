<template>
    <div class="message-container">
       <p>{{ msg }}</p>
    </div>
</template>

<script>
export default {
    name: "Message",
    props: {
        msg: String
    }
}
</script>

<style scoped>
.message-container {
    color:#222;
    font-weight: bold;
    background-color: #fcba0396;
    backdrop-filter: blur(5px);
    border: 2px solid #e1af23;
    border-radius: 5px;
    padding: 10px;
    max-width: 500px;
    margin: 30px auto;
    text-align: center;
}

</style>