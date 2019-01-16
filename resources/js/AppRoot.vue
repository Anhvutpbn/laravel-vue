<template>
    <div>
        <app-header></app-header>
        <router-view></router-view>

    </div>
</template>

<script>
    import Header from "./components/Header"
    export default {
        components: {
            'app-header' : Header
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
                // alert(title)
            }
        }
    }
</script>
