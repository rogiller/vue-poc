<template>
  <div class="first">
    <b>{{message}}</b>
    <div>
      <input type="text" v-model="textValue"/>
      <input type="button" value="OK" v-on:click="onBtnClick"/>
    </div>
  </div>

</template>

<script>
export default {
  name: 'First',
  data () {
    return {
      btnText: 'OK',
      textValue: '',
      message: 'First!'
    }
  },
  methods: {
    onBtnClick: function (event) {
      alert(this.textValue)
      this.textValue = ''
    }
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
