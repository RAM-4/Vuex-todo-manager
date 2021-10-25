<template>
  <div id="app">
    <div class="container">
      <add-todos/>
      <filter-todos/>
      <todos/>
    </div>
  </div>
</template>

<script>
import Todos from './components/Todos.vue'
import AddTodo from './components/AddTodo.vue'
import FilterTodos from './components/FilterTodos.vue'

export default {
  name: 'App',
  components: {
    'todos': Todos,
    'add-todos': AddTodo,
    'filter-todos': FilterTodos
  }
}
</script>

<style>
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  line-height: 1.6;
  background: #e8f7f0;
}
.container {
  max-width: 1100px;
  margin: auto;
  overflow: auto;
  padding: 0 2rem;
}
</style>
