<template>
  <div>
    <input v-model="text" placeholder="Type here">
    <p>{{ text }}</p>
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
export default {
  data () {
    return {
      text: ''
    }
  },
  methods: {
    onInput (e) {
      this.text = e.target.value
    }
  }
}
</script>
