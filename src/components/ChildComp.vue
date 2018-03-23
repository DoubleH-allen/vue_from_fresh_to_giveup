<template>
  <div class="chik">
    <input ref="aabb" v-model="msg" :placeholder=Testdata v-on:change="funca">
  </div>
</template>

<script>
export default {
  name: 'ChildComp',
  props: ['Testdata'],
  data () {
    return {
      msg: ''
    }
  },
  methods: {
    funca: function () {
      console.log(this.msg + 'this')
      console.log(this.$refs.aabb.placeholder)
      this.$emit('funcaaaa', this.msg)
    },
    afucn: function () {
    	console.log(this.aDouble, 'aaa')
    	this.$refs.aabb.placeholder = this.aDouble
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scope></style>
