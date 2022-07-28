<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: { HelloWorld }
}
</script>

<template>

  <article>
    <div class="cell small red">
      <h1>Welcome on my portfolio</h1>
    </div>

    <div class="cell big black">
      <img src="/vite.svg" alt="Vite logo" width="50%" style="">
      <img src="src/assets/vue.svg" alt="Vite logo" width="50%" style="">
    </div>
  </article>

  <article>
    <div class="cell big white">
      <p>There will be good stuff in here !</p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
        beatae quia voluptatem tenetur temporibus quibusdam doloribus !
      </p>
    </div>

    <div class="cell small red">
      <p>Lorem ipsum dolor sit amet.</p>
    </div>
  </article>

  <article>
    <div class="cell small red">
      <p>There will be good stuff in here !</p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
        beatae quia voluptatem tenetur temporibus quibusdam doloribus !
      </p>
    </div>

    <div class="cell big black">
      <p>Lorem, ipsum dolor.</p>
    </div>
  </article>

</template>

<style scoped>
</style>
