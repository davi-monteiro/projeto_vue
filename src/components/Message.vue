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
        color: #004085;
        text-align: center;
        background: #CCE5FF;
        border: 2px solid #B8DAFF;
        border-radius: 5px;
        padding: 10px;
        width: 100%;
        margin: 30px 0;
    }
</style>