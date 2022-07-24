<template>
  <div class="hello">
    <h1>1</h1>
    <div v-for="(item, index) in my_forms" :key="index">
       <span v-if="item.name">name:<a id="name">{{ item.name }}</a></span>
    </div>
    <div class="v_model">
      <h1>2</h1>
      <input v-model="messg">
      <p>Message is {{messg}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      messg: 'dedededed',
      my_forms: [{ name: 'wanzi' }, { name: 'shuying' }, { age: 18 }]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#name {
  color: blue;
}
.hello {
background-color: rgb(214, 208, 219);
border: 1px solid ;
}
</style>
