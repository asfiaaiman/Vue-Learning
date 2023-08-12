<!-- We will call this in App.vue -->

<template>
    <h2>I am parent </h2>
    <ChildComponent/>
</template>

<script>

// Calling child component here
import ChildComponent from '../components/child.vue'


export default {
    name: 'Parent',
    components: {
        ChildComponent
    }
}
</script>