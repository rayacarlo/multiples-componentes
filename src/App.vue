<template>

  <div id="app">
    <img alt="Vue logo" src="./assets/banner.png">
    <HelloWorld msg="Things that I want to learn vs. things that I already learnt this year"/>
    <ThingstoLearn title="5 things that I want to learn" v-bind:links="things_to_learn" />
    <ThingstoLearn title="5 things that I already learnt" v-bind:links="things_learnt" />
  </div>

</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import ThingstoLearn from './components/ThingstoLearn.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ThingstoLearn
  },
  data: () => {
    return {
      things_to_learn: [
        {
          text: 'UX/UI',
          url: 'https://www.skillshare.com/classes/Designing-for-the-Future-UIUX-Prototyping/915958036?via=search-layout-grid'
        },
        {
          text: 'SVG',
          url: 'https://www.skillshare.com/classes/Creative-Coding-Animating-SVG-with-Simple-CSS-Code/1735436116?via=search-layout-grid'
        },
        {
          text: 'Typography',
          url: 'https://www.skillshare.com/classes/How-to-Look-at-Type-Fundamentals-of-Web-Typography/246544835?via=search-layout-grid'
        },
        {
          text: 'Accesibility',
          url: 'https://www.skillshare.com/classes/Inclusive-UX-Designing-Websites-for-Everyone/297973484?via=search-autocomplete'
        },
        {
          text: 'Motion Graphics',
          url: 'https://www.skillshare.com/classes/Introduction-to-Adobe-After-Effects-Getting-Started-with-Motion-Graphics/1983581210?via=search-autocomplete'
        }
      ],
      things_learnt: [
        {
          text: 'HTML',
          url: 'https://learn.codingdojo.com/m/122/6238'
        },
        {
          text: 'CSS',
          url: 'https://learn.codingdojo.com/m/122/6239'
        },
        {
          text: 'Javacript',
          url: 'https://learn.codingdojo.com/m/122/6240'
        },
        {
          text: 'jQuery',
          url: 'https://learn.codingdojo.com/m/122/6258'
        },
        {
          text: 'Github',
          url: 'https://learn.codingdojo.com/m/151/6266'
        }
      ]
    }
  }
}

</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}

</style>
