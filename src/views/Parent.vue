<!-- We will call this in App.vue -->

<template>
    <!-- I am getting the value of prop here that I hace defined in ChildComponent -->
    <ChildComponent :childName="parentName" :clickFunction="alertFunction"/>
</template>

<script>

// Calling child component here
import ChildComponent from '../components/child.vue'


export default {
    name: 'Parent',
    components: {
        ChildComponent
    },
    // Data is access by data()
    data()
    {
        return{
            parentName: "Hi there, Asfia"
        }   
    },
    methods:
    {
        // Defining functions here
        alertFunction()
        {
            alert('I am function');
        }
    }
}
</script>