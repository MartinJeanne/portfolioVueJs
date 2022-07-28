<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: { HelloWorld }
}
</script>

<template>

  <header class="grid last-big">
    <div class="cell red">
      <h1>Welcome on my portfolio</h1>
    </div>

    <div class="cell black">
      <img src="src/assets/pp_cool.jpg" alt="Photo de profil">
    </div>
  </header>

  <article class="grid first-big">
    <div class="cell white">
      <p>There will be good stuff in here !</p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
        beatae quia voluptatem tenetur temporibus quibusdam doloribus !
      </p>
    </div>

    <div class="cell red">
      <p>Lorem ipsum dolor sit amet.</p>
    </div>
  </article>

  <footer class="grid last-big">
    <div class="cell red">
      <p>There will be good stuff in here !</p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
        beatae quia voluptatem tenetur temporibus quibusdam doloribus !
      </p>
    </div>

    <div class="cell black">
      <p>Lorem, ipsum dolor.</p>
    </div>
  </footer>

</template>

<style scoped>
</style>
