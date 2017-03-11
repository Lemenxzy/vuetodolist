<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: 'hello',
  data () {
    return {
      msg: 'LOVE TO DO LIST!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="sass" rel="stylesheet/sass">
  .hello
    text-align: center
    h1, h2
      font-weight: normal

</style>
