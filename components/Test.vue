<template>
  <div>
    <h1>{{ message }}</h1>
    <p>Count is: {{ counter.count }}</p>
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
      message: 'Hello World',
      counter: {                               // НЕ МОГУ ПОНЯТЬ ДЛЯ ЧЕГО НУЖНЫ 22 и 23 строка ( без них не работает )
        count: 0
      }
    }
  }
}
</script>
