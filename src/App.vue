<template>
  <div id="app">
    <my-slot>
      <my-component :symbol="mySymbol"></my-component>
    </my-slot>
  </div>
</template>

<script>
import MySlot from './components/MySlot.vue'
import MyComponent from './components/MyComponent.vue'

export default {
  name: 'app',
  components: {
    MySlot,
    MyComponent,
  },
  data () {
    return {
      mySymbol: Symbol('MINE')
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
