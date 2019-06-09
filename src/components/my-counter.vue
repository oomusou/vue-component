<template>
  <div>
    <span>{{ counter }}</span>
    <p></p>
    <button @click="add">+1</button>
  </div>
</template>

<script>
let add = function() {
  this.counter++;
};

export default {
  name: 'my-counter',
  data: () => ({ counter: 0}),
  methods: { add }
}
</script>
