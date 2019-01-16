<template>
    <div>
        <button @click="component = 'app-home'">Home</button>
        <button @click="component = 'app-contact'">Contact</button>

        <app-header></app-header>
        <component v-bind:is="component" v-bind:component="component" @changeTitle="changeTitle"></component>
        <app-footer></app-footer>
    </div>
</template>

<script>
    import Header from "./components/Header"
    import Footer from "./components/Footer"
    import Contact from "./components/pages/Contact"
    import Home from "./components/pages/HomePage"
    export default {
        components: {
            'app-home': Home,
            'app-footer' : Footer,
            'app-header' : Header,
            'app-contact': Contact
        },
        mounted() {
            console.log('Component mounted.')
        },
        data() {
            return {
                component: 'app-home'
            }
        },
        methods: {
            changeTitle(title) {
                alert(title)
            }
        }
    }
</script>
