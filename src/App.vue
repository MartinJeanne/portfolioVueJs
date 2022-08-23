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
    <p>Welcome on the portfolio of a junior developper (i know it doesn't seem to be)</p>
    
  </header>

  <article class="tall white">
    <h2>Projects</h2>
    <p>
      There's a list of projects that i participed to !
    </p>
  </article>

  <article class="medium red">
    <h2>Free</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </article>

  <div class="tall black">
    <h2>Photo + contact</h2>
    <img
      src="src/assets/pp_cool.jpg"
      alt="Photo Martin"
      width="1196"
      height="2301"
    />
  </div>

  <footer class="medium black">
    <h2>Footer</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit
      beatae quia voluptatem tenetur temporibus quibusdam doloribus !
    </p>
  </footer>

  <article class="short red">
    <h2>Skills</h2>
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
