<template>
  <div class="hello">
    <h1> Input String </h1>
   <input type="text" v-model="take" >
   <p>Output .....</p>
   <h1> {{ output }}</h1>
  </div>


</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      take : ''
    }
  },
  computed :{
    output : function(){
      return this.take.toUpperCase();
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
