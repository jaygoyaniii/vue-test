<template>
    <h4>Class Binding</h4>
    <h2 class="otherclass" :class="{ green: colorfull }"> Home Component </h2>
    <button v-on:click="colorfull = !colorfull">Apply Style</button>
</template>

<script>
export default {
        name: "ClassBinding",
    data() {
        return {
            colorfull: false
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}

.green {
    background-color: green;
    width: 200px;
    padding: 10px;
}
</style>