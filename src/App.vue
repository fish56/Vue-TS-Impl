<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Model/>
    <Template/>
    <Event/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Model from './components/model/Index.vue';
import Template from './components/template/Index.vue';
import Event from './components/events/Index.vue';

@Component({
  components: {
    Model,
    Template,
    Event
  },
})
export default class App extends Vue {}
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
