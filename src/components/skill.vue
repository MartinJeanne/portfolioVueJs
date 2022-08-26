<script>
import { onMounted, ref } from 'vue'

export default {
  components: {},

  props: {
    skill: String,
    value: Number,
    color: String
  },

  setup(props) {
    const progress = ref(null);

    onMounted(() => {
      let c = progress.value.classList;

      switch (props.color) {
        case 'red':
          c.add('red'); break;
        case 'yellow':
          c.add('yellow'); break;
        case 'purple':
          c.add('purple'); break;
      }
    });

    return { progress }
  }
}
</script>

<template>
  <div class="skill">
    <p>{{ skill }}</p>
    <progress ref="progress" :value="value" max="100"></progress>
  </div>
</template>

<style scoped>
.skill {
  width: 500px;
  margin-left: 16px;
  margin-bottom: 12px;
  display: flex;
  justify-content: space-between;
}

p {
  margin-right: 16px;
  letter-spacing: 1px;
  font-weight: 300;
  font-size: 1.1em;
  text-transform: uppercase;
}

progress {
  height: 14px;
  width: 350px;
  border-radius: 8px;
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);

}

progress::-webkit-progress-bar {
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.25) inset;
  background: #f7f7ff;
}

progress::-webkit-progress-value {
  border-radius: 8px;
}

/* List of color */
.red::-webkit-progress-value {
  background-image:
    -webkit-linear-gradient(top, rgba(255, 255, 255, .1), rgba(0, 0, 0, .1)),
    -webkit-linear-gradient(left, #ef233c, #ef233c);
}

.yellow::-webkit-progress-value {
  background-image:
    -webkit-linear-gradient(top, rgba(255, 255, 255, .1), rgba(0, 0, 0, .1)),
    -webkit-linear-gradient(left, #efca23, #f3c33e);
}

.purple::-webkit-progress-value {
  background-image:
    -webkit-linear-gradient(top, rgba(255, 255, 255, .1), rgba(0, 0, 0, .1)),
    -webkit-linear-gradient(left, #a423ef, #bf40f1);
}
</style>
