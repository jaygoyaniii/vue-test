<template>
    <h4>Parent Component</h4>
    <ChildComponent name="Jay" :user="user" :getData="getData" />
</template>

<script>
import ChildComponent from './ChildComponent.vue';

export default {
    name: "ParentComponent",
    components: {
        ChildComponent
    },
    data() {
        return {
            user: { name: 'Thomas', email: 'thomas@gmail.com' }
        };
    },
    methods: {
        getData() {
            console.warn("Parent function called");
            alert("Hello")
        }
    }
}
</script>
