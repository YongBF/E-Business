<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
@import url('//at.alicdn.com/t/font_960852_gft8etvzmid.css');
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.small-icon {
  font-size: 0.8rem;
}

.normal-icon {
  font-size: 1rem;
}

.large-icon {
  font-size: 1.3rem;
}
</style>
