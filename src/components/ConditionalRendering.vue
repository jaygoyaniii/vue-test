<template>
    <h3 v-if="show">if condition</h3>
    <!-- <h3 v-else>else condition</h3> -->
    <button v-on:click="show = !show">Show</button>
</template>

<script>
    export default {
        name: "ConditionalRendering",
        data() {
            return {
                show:true
            }
        }
    }
</script>