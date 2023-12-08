<script>
export default {
    data: () => ({
        contador: 10
    }),
    methods: {
        sumar() {
            this.contador++
        },
        restar() {
            this.contador--
        },
        reset() {
            this.contador = 10
        },
    },
}
</script>

<template>
    <div class="container">
        <img src="./assets/logo.png" alt="logo vue" width="125" height="125">
        <h1>CRM Vue 3</h1>
        <hr />

        <small>
            <h2>Contador: {{ contador }}</h2>
        </small>

        <button @click="sumar()">+1</button>
        <button @click="restar()">-1</button>
        <button @click="reset()">Reset</button>
    </div>
</template>
<style scoped>
.container {
    text-align: center;
}

h1 {
    color: red;
}

small {
    color: #666;
    font-size: 2.5rem;
}

button {
    color: blue;
    font-size: 1.5rem;
    margin: 0px 6px;
}
</style>