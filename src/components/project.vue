<script>
import { ref } from 'vue'

export default {
  components: {},

  props: {
    title: String,
    desc: String,
    src: String
  },

  setup(src) {
    src = 'test/' + src
    const count = ref(0)
    const test = ref()

    return { count }
  }
}
</script>

<template>
  <div class="project">
    <img :src="src" :alt="title" />
    <p>My project : {{ title }}, {{ desc }}, {{ src }}</p>
  </div>
</template>

<style scoped>
.project {
  display: flex;
  flex-direction: column;
  background: rgb(190, 190, 190);
}
</style>
