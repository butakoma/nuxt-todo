<template>
  <div class="container">
    <div class="columns">
      <div class="column">
        <card v-bind:todos="todos"></card>
      </div>
    </div>
  </div>
</template>

<script>

import Card from '~/components/Card.vue'

export default {
  components: {
    Card
  },
  data () {
    return {
      todos: [{
        title: 'title A',
        text: 'text A',
        status: 'doing'
      }]
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
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
