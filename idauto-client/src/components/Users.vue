<template>
    <div>
    <b-card title="User Lookup" sub-title="subtitle">
    <b-card-text>
      Some quick example text to build on the <em>card title</em> and make up the bulk of the card's
      content.
    </b-card-text>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <li>{{todo.title}}</li>
            <TodoItem v-bind:todo="todo" />
        </div>
            <b-card-text>A second paragraph of text in the card.</b-card-text>

    <a href="#" class="card-link">Card link</a>
    <b-link href="#" class="card-link">Another link</b-link>
  </b-card>
    </div>
</template>

<script>
export default {
    name: "Todos",
    props: ["todos"]
}
</script>

<style scoped>
    li {
        background: white;
    }
</style>