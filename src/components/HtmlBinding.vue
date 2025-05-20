<template>
    <h3>HTML Binding</h3>
    <h4>{{ text }}</h4>
    <div v-html="tag"></div>
</template>


<script>
export default {
    name: "HtmlBinding",
    data() {
        return {
            text: "John Doe",
            tag: "<h1>Good Morning</h1>"
        }
    }
}   
</script>