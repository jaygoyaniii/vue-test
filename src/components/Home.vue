<template>
    <div>
        <h1>Home Component</h1>
        <h2>Email: {{ email }}</h2>
        <h4>Mobile: {{ mobile }} </h4>
        <h4>Name: {{ getName() }}</h4>
        <div style="margin: 20px 0;">
            <button @click="decrementCount">-</button>
            <span style="margin: 0 10px;">{{ count }}</span>
            <button @click="incrementCount">+</button>
        </div>
        <input type="text" v-model="count">

        <h1>Get Input field value</h1>
        <input type="text" placeholder="Enter your email" v-model="Email">
        <br><br>
        <input type="password" placeholder="Enter your password" v-model="password">
        <br><br>
        <button v-on:click="getData()" type="button">Get Values</button>
    </div>
</template>

<script>
export default {
    name: 'HomeComponent',
    data() {
        return {
            email: 'test@gmail.com',
            mobile: 8123456789,
            count: 0,
            Email: null,
            password: null
        }
    },
    methods: {
        getName() {
            return "Jay Goyani"
        },
        incrementCount() {
            this.count += 1;
        },
        decrementCount() {
            if (this.count > 0) {
                this.count -= 1;
            }
        },
        getData() {
            console.warn("values:", this.Email, this.password);
        }
    }
}
</script>