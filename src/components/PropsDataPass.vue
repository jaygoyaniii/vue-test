<template>
    <h1>Props Data Passing</h1>
    <Student :name="name" />
    <Teacher name="Peter" />
</template>

<script>
import Student from './Student.vue';
import Teacher from './Teacher.vue';

export default {
    name: "PropsDataPass",
    data() {
        return {
            name: "Bruce Lee"
        }
    },
    components: {
        Student,
        Teacher
    }
}
</script>