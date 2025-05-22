<template>
    <h1>Send Data Child to Parent in VueJS</h1>
    <User :getUser="getUserName" />
</template>


<script>
import User from './User.vue';

export default {
    name: "ChildParentData",
    components: {
        User
    },
    methods: {
        getUserName(name) {
            alert(name)
        }
    }
}
</script>