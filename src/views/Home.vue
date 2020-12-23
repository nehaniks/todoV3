<template>
  <div class="home">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from "../components/Todos";

export default {
  name: 'Home',
  components: {
    Todos
  },
  setup() {
    let todos = [
      {
        id: 1,
        title: 'Todo One',
        completed: true
      },
      {
        id: 2,
        title: 'Todo Two',
        completed: false
      },
      {
        id: 3,
        title: 'Todo Three',
        completed: true
      }
    ]
    return {
      todos
    }
  }
}
</script>
