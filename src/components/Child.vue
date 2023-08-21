<template>
    <!-- I am calling the prop here -->
    <h1>Welcome {{ childName }}</h1>
    <button v-on:click="clickFunction">Click Here</button>
</template>

<script>

//We register components in the script tag

export default{
    //The functions, varibales, and events here will be exported to other files
    name: 'ChildComponent',
    // Props have those variables that we will use in this file. We will send these variables to other files
    props: {
        childName: String,
        clickFunction: Function,
    },
    
}
</script>