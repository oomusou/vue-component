<template>
  <div>
    <button @click="onSelectLesson">Lessons</button>
    <button @click="onSelectApply">Apply</button>
    <p></p>
    <keep-alive>
      <component :is="content"></component>
    </keep-alive>
  </div>
</template>

<script>
import myLessons from './components/my-lessons.vue';
import myApply from './components/my-apply.vue';

let onSelectLesson = function() {
  this.content = 'my-lessons';
};

let onSelectApply = function() {
  this.content = 'my-apply';
};

export default {
  name: 'app',
  components: {
    myLessons,
    myApply
  },
  data: () => ({ content: 'my-lessons' }),
  methods: {
    onSelectLesson,
    onSelectApply,
  }
};
</script>
