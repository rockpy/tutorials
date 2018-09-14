<template>
  <div id="app">
    <header>
        <h1>Header</h1>
    </header>
    <div id="grid2">
        <Menu msg="app" />
        <Content msg="" />
    </div>
    <footer>
        <h6>footer</h6>
    </footer>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #1D293C;
}

*{
    margin: 0;
    padding: 0;
}
body{
    background: #1D293C;
}
header{    
    min-height: 60px;
    color: #23FF0C;
    padding: 10px 0 0 10px;
}

footer{
    min-height: 160px;
    color: #23FF0C;
    padding: 10px 0 0 10px;
}

#grid2 {
    display: grid;
    grid-template-columns: 1fr 5fr;

}
</style>

<script>
import Menu from './components/menu.vue'
import Content from './components/content.vue'

export default {
  name: 'app',
  components: {
    Menu,
    Content
  }
}
</script>