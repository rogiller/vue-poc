<template>
  <div class="first">
    <b>{{message}}</b>
    <div>
      <input type="text"/>
      <input type="button" value="OK"/>
    </div>
  </div>

</template>

<script>
export default {
  name: 'First',
  data () {
    return {
      btnText: 'OK',
      message: 'First!'
    }
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
