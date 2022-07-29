<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: { HelloWorld }
}
</script>

<template>
  <header class="short red">
    <h1 id="myName">Martin</h1>
    <h1 id="portfolio">Portfolio</h1>
  </header>

  <article class="tall white">
    <p>There will be good stuff in here !</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </article>

  <article class="short red">
    <p>There will be good stuff in here !</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </article>

  <div class="tall black">
    <img
      src="src/assets/pp_cool.jpg"
      alt="Photo Martin"
      width="1196"
      height="2301"
    />
  </div>

  <footer class="tall black">
    <p>There will be good stuff in here !</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </footer>

  <article class="short red">
    <p>There will be good stuff in here !</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </article>
</template>

<style scoped>
#myName {
  letter-spacing: 4px;
}

#portfolio {
  font-weight: 400;
}
</style>
