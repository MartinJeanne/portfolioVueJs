<script>
import HelloWorld from './components/HelloWorld.vue'
import Project from './components/Project.vue'
import Skills from './components/Skill.vue'
import Skill from './components/Skill.vue';

export default {
  components: { HelloWorld, Project, Skill, Skill }
}
</script>

<template>
  <header class="short red">
    <h1 id="myName">Martin</h1>
    <h1 id="portfolio">Portfolio</h1>
    <p>
      Welcome on the portfolio of a junior developper (i know it doesn't seem to
      be)
    </p>
  </header>

  <article class="tall white">
    <h2>Projects</h2>
    <p>There's a list of projects that i participed to !</p>
    <Project title="My awsome project" desc="This is my best project !" img="vite.svg" />
    <Project title="My awsome project" desc="This is my best project !" img="vite.svg" />
    <Project title="My awsome project" desc="This is my best project !" img="vite.svg" />
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
    <img src="src/assets/pp_cool.jpg" alt="Photo Martin" width="1196" height="2301" />
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
    <Skill skill="html & css" value="80" color="red"/>
    <Skill skill="php" value="45" color="purple"/>
    <Skill skill="JavaScript" value="70" color="yellow"/>
  </article>
</template>

<style scoped>
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: 20% 50%;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  filter: grayscale(100%) contrast(170%);
}

#myName {
  letter-spacing: 4px;
}

#portfolio {
  font-weight: 400;
}
</style>
