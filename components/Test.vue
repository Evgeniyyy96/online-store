<template>
  <div>
    <button @click="toggle">toggle</button>
    <h1 v-if="awesome">Vue is awesome!</h1>
    <h1 v-else>Oh no 😢</h1>
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
      awesome: true
    }
  },
  methods: {
    toggle () {
      this.awesome = !this.awesome
    }
  }
}
</script>
