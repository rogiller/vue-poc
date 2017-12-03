<template>
  <div class="first">
    <b>{{message}}</b>
  </div>
</template>

<script>
export default {
  name: 'First',
  data () {
    return {
      message: 'First [from data]'
    }
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
