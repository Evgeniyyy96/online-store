<template>
  <div>
  <input v-model="newTodo" @keyup.enter="addTodo">
  <button @click="addTodo">Add Todo</button>
  <ul>
    <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
      <button @click="removeTodo(todo)">X</button>
    </li>
  </ul>
  </div>
</template>

<script>
export default {
  name: 'NameComponent',
  data () {
    return {}
  }
}
</script>

<script>
let id = 0

export default {
  data() {
    return {
      newTodo: '',
      todos: [
        { id: id++, text: 'Learn HTML' },
        { id: id++, text: 'Learn JavaScript' },
        { id: id++, text: 'Learn Vue' }
      ]
    }
  },
  methods: {
    addTodo () {
      this.todos.push({ id: id++, text: this.newTodo })
      this.newYodo = ''
    },
    removeTodo(todo) {
      this.todos = this.todos.filter((t) => t !== todo)       // Не поня как фильтр сделан
    }
  }
}
</script>
