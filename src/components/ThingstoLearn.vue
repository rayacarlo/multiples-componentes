<template>

  <div>
    <h1>{{ title }}</h1>
    <ul>
      <li v-for="(link, i) in links" v-bind:key="i"><a v-bind:href="link.url">{{ link.text }}</a></li>
    </ul>
  </div>

</template>

<script>

export default {
  name: 'ThingstoLearn',
  props: {
    title: String,
    links: Array
  }
}
</script>

<style scoped>

h1 {
  margin: 40px 0 0;
  font-size: 16px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

</style>