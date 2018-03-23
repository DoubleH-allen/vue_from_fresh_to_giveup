<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <TestTest :Testdata='msg' />
    <input v-model="message" placeholder="edit me" >
    <p>Message is: {{ message }}</p>
    <ChildComp :Testdata='message' v-on:funcaaaa="getfunca" />
  </div>
</template>

<script>
import ChildComp from '@/components/ChildComp'
import TestTest from '@/components/TestTest'
export default {
  name: 'HelloWorld',
  data () {
    return {
      message: 'Welcome to Your Vue',
      msg: 'what the fuck!'
    }
  },
  components: {
    TestTest,
    ChildComp
  },
  methods: {
    getfunca: function (aaa) {
      console.log(aaa)
      this.message = aaa
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-size: 30px;
}
</style>
