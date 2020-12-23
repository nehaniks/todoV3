<template>
    <div>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <h1>{{ todo.title }}</h1>
        </div>
    </div>
</template>

<script>
export default {
    name: "Todos",
    props: {
        todos: {
            required: true,
            type: Object
        }
    }
    // setup(props) {
    //     let todos = []
    //     return {

    //     }
    // }
}
</script>

<style scoped>

</style>