<script>
import { ref } from 'vue'

export default {
  components: {},

  props: {
    skill: String,
    value: Number,
    img: String
  },

  setup(props) {
    const src = ref('skill/' + props.img);
    return { src }
  }
}
</script>

<template>
  <div class="skill">
    <p>{{skill}}</p>
    <progress :value="value" max="100">Hello</progress>
  </div>
</template>

<style scoped>
.skill {
  width: 37vw;
  margin: auto;
  display: flex;
  justify-content: space-between;
  margin-bottom: 12px;
}

p {
  margin-right: 16px;
  letter-spacing: 1px;
  font-weight: 300;
  font-size: 1.1em;
  text-transform: uppercase;
}

progress {
  border-radius: 6px;
  width: 30vw;
  height: 20px;
  box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.2);
}

progress::-webkit-progress-bar {
  background-color: #eee;
  border-radius: 6px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.25) inset;
}

progress::-webkit-progress-value {
  background-image:
    -webkit-linear-gradient(-45deg, transparent 33%, rgba(0, 0, 0, .1) 33%, rgba(0, 0, 0, .1) 66%, transparent 66%),
    -webkit-linear-gradient(top, rgba(255, 255, 255, .25), rgba(0, 0, 0, .25)),
    -webkit-linear-gradient(left, rgb(204, 0, 0), #f44);
  border-radius: 6px;
  background-size: 35px 20px, 100% 100%, 100% 100%;
}
</style>
