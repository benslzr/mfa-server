<template>
    <div>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <h3>{{todo.title}}</h3>
            <TodoItem v-bind:todo="todo" />
        </div>
    </div>
</template>

<script>
export default {
    name: "Todos",
    props: ["todos"]
}
</script>

<style scoped>
    h3 {
        background: white;
    }
</style>