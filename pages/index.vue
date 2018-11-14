<template>
  <section class="container">
    <div>
      <Header />
      <no-ssr> 
        <carousel>
          <slide>
            Slide 1 Content
          </slide>
          <slide>
            Slide 2 Content
          </slide>
          <slide>
            Slide 3 Content
          </slide>
          <slide>
            Slide 4 Content
          </slide>
          <slide>
            Slide 5 Content
          </slide>

        </carousel>
      </no-ssr>
      <h1 class="title">
        adoptMe
      </h1>
      <h2 class="subtitle">
        website template for local pet adoption businesses
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green">Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey">GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/header.vue'
// import { Carousel, Slide } from 'vue-carousel'
import NoSSR from 'vue-no-ssr';

// let pluginLib;

// if (process.browser) {
//   pluginLib = require('vue-carousel');
// }

export default {
  components: {
    Logo,
    Header,
    // Carousel,
    // Slide,
    'no-ssr': NoSSR
  },
  // mounted() {
  //   console.log(pluginLib);
  // }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
