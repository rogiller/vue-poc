<template>
  <div class="first">
    <div>
      <el-input placeholder="Please input message..." v-model="textValue"></el-input>
      <el-button type="primary" v-on:click="onBtnClick">DONE</el-button>
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
      this.$alert(this.textValue, 'Message', {
        confirmButtonText: 'OK'
      })
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
