<template>
    <div class="todo-item" v-bind:class="{'is-complete':todo.complete}">
        <p>Todo Item</p>
        <p>{{todo.title}}</p>
    </div>
</template>

<script>
export default {
    name:"TodoItem",
    props: ["todo"],
    methods: {
        markComplete() {
            this.props 
        }
    }
}
</script>

<style scoped>
 .todo-item{
     background: lightgrey;
     padding: 10px;
     border-bottom: 1px #ccc dotted;
 }

 .is-complete {
     text-decoration:  line-through;
    }

 .del {
     background: red;
     color: white;
 }
</style>