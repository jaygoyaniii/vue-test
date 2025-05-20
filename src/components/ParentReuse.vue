<template>
    <h3>Parent Component</h3>
    <ul>
        <li v-for="item in users" :key="item.name">
            <ChildReuse :data="item" :getData="() => getData(item.name)" />
        </li>
    </ul>
</template>

<script>
import ChildReuse from './ChildReuse.vue';

export default {
    name: "ParentReuse",
    components: {
        ChildReuse
    },
    methods: {
        getData(name) {
            alert(name)
        }
    },
    data() {
        return {
            users: [
                { name: 'John Doe', email: 'johndoe@gmail' },
                { name: 'Peter Role', email: 'peterrole@gmail' },
                { name: 'Keneth Kole', email: 'kenethkole@gmail' },
            ]
        }
    }
}
</script>