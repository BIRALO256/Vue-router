<template>
    <h1>Lectures details Page</h1>
    <p>the lecture id is {{ id }}</p>
</template>

<script>
export default {
    props:['id'],
    data(){
        // id:this.$route.params.id
    }
}
</script>

<style>

</style>