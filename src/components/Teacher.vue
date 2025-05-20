<template>
    <h3>Teacher Name is : {{ name }}</h3>
</template>



<script>
export default {
    name: 'TeacherComponent',
    props: {
        name: String
    }
}
</script>