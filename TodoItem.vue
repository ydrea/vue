<template>
    <div> 
    <div> 
 <h4> {{todo.title}}</h4>
    </div> 
</div> 

    </template>

<script>
export default {
    name: "TodoItem",
    props: ["todo"]
}
</script>

<style scoped>

</style>