<template>
    <div class="container">
        <h1>Malesef Bilemediniz!!!</h1>
        <button @click="newGame">Yeni Oyun</button>
    </div>
</template>

<script>
export default {
    methods : {
        newGame() {
            this.$emit("activeComponentEvent", "app-game-cards");
        }
    }
}
</script>

<style scoped>

    .container {
        width: 100%;
        height: 100vh;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: darkred;
    }

    .container h1 {
        text-align: center;
        font-size: 333%;
        color: #fff;
    }

    .container button {
        width: 200px;
        background-color: #fff;
        color: darkred;
        border: 1px solid brown;
        height: 50px;
        font-size: 15px;
        border-radius: 5px;
        outline: none;
        transition: all .5s;
        cursor: pointer;
    }

    .container button:hover {
        background-color: lightgreen;
        color: #fff;
        transition: all .5s;
    }

</style>

