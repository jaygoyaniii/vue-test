<template>
    <h1>Send Data Child to Parent in VueJS</h1>
    <h4>{{ childUser }}</h4>
    <User :getUser="getUserName" />
</template>


<script>
import User from './User.vue';

export default {
    name: "ChildParentData",
    data() {
        return {
            childUser: ""
        }
    },
    components: {
        User
    },
    methods: {
        getUserName(name) {
            this.childUser = name
        }
    }
}
</script>