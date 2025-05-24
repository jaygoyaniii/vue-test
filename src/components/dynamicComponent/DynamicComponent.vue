<template>
    <h3>Dynamic Component</h3>
    <button @click="tab = 'NodeComponent'">Load Node Component</button>
    <button @click="tab = 'PhpComponent'">Load PHP Component</button>
    <button @click="tab = 'JavaComponent'">Load Java Component</button>
    <component :is="tab"></component>
</template>

<script>
import NodeComponent from './Node.vue';
import PhpComponent from './Php.vue';
import JavaComponent from './Java.vue';
export default {
    name: "DynamicComponent",
    components: {
        NodeComponent,
        PhpComponent,
        JavaComponent
    },
    data() {
        return {
            tab: 'NodeComponent'
        }
    }
}
</script>