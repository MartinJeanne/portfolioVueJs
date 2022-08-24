<script>
import { ref } from 'vue'

export default {
  components: {},

  props: {
    title: String,
    desc: String,
    img: String
  },

  setup(props) {
    const src = ref('project/' + props.img);

    return { src }
  }
}
</script>

<template>
  <div class="project">
    <img :src="src" :alt="title" />
    <p>{{ title }}: {{desc}}</p>
  </div>
</template>

<style scoped>

p {
  margin: 0;
  font-size: 1.3em;;
}

.project {
  display: flex;
  flex-direction: row;
  align-items: center;
  border-radius: 8px;
  margin-top: 16px;
  box-shadow: 1px 1px 5px rgba(0, 0, 0, 0.2);
  background: rgba(0, 0, 0, 0.1);
}

.project>img {
  width: 65px;
  height: 65px;
  border-radius: 50%;
  margin: 8px 16px 8px 8px;
}
</style>
