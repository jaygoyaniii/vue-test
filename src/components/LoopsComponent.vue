<template>
    <h3>Loops in VueJS</h3>
    <ul>
        <li v-for="(item, index) in technology" :key="index"> {{ item }}</li>
    </ul>
    <br> <br>
    <ul>
        <li v-for="(user, index) in users" :key="index">
            {{ user.name }} - {{ user.email }}
        </li>
    </ul>
</template>

<script>
export default {
    name: "LoopsComponent",
    data() {
        return {
            technology: ['java','php','node','python'],
            users: [{
                name: "Jay",
                email: "jaytest@gmail.com"
            },
            {
                name: "Peter",
                email: "peter@gmail.com"
            },
            {
                name: "Thomas",
                email: "thomas@gmail.com"
            }]
        }
    }
}
</script>

