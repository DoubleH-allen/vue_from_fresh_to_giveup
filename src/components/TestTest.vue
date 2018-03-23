<template>
  <div class="TestTest">
    <h1>{{ Testdata }}</h1>
  </div>
</template>

<script>
export default {
  name: 'TestTest',
  props: ['Testdata'],
  data () {
    return {
      msg: 'aaaaa'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scope></style>
