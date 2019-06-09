<template>
  <div>
    <my-counter></my-counter>
    <p></p>
    <my-counter></my-counter>
  </div>
</template>

<script>
import myCounter from './components/my-counter.vue'

export default {
  name: 'app',
  components: {
    myCounter
  }
}
</script>
