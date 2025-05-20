<template>
    <h2>Get CustomCheckbox & Radio Button Value</h2>
    <h3>Technology</h3>
    <input type="checkbox" id="java" value="java" v-model="technology">
    <label for="java">Java</label>

    <input type="checkbox" id="php" value="php" v-model="technology">
    <label for="php">PHP</label>

    <input type="checkbox" id="node" value="node" v-model="technology">
    <label for="node">Node</label>

    <h4>Selected Technology: {{ technology }}</h4>
</template>

<script>
export default {
    name: 'CustomCheckbox',
    data() {
        return {
            technology: []
        }
    }
}
</script>
