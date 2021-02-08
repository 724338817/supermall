<template>
  <div id="app">
    <router-view/>
      <main-tar-bar/>
  </div>
</template>

<script>
import mainTarBar from "components/content/mainTarBar/mainTarBar"

export default {
  name: 'App',
  components: {
    mainTarBar
  }
}
</script>
<style>
@import "assets/css/base.css";
</style>
