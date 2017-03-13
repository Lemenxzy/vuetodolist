<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: 'app'
}
</script>

<style  lang="sass" rel="stylesheet/sass">
  html,body,#app
    height: 100%
    @import "common/fonts/style.css"
</style>
