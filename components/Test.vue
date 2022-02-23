<template>
  <div>
    <h1 :class="titleClass">Make me red</h1>
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
      titleClass: 'title'
    }
  }
}
</script>

<style>
.title {
  color: red;
}
</style>
