<template>
  <div id="app">
    <NavBar />
    <router-view/>
  </div>
</template>
<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import NavBar from '@/components/NavBar.vue' // @ is an alias to /src

@Component({
  components: {
    NavBar
  }
})
export default class App extends Vue {}
</script>
<style lang="scss">
body {
  min-height: calc(100vh - 100px);
  #app {
    font-family: pictos, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  ul,
  li {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  video {
    max-width: 100%;
  }
}
</style>
