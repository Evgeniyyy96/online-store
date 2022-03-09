<template>
  <div>
    <button @click="increment">count is: {{ count }}</button>
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
      count: 0
      }
    }
  }
</script>

<script>
export default {
  data () {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      this.count++
    }
  }
}
</script>
