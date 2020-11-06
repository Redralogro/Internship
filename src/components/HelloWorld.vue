<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button v-on:click="Add(10)" >Add </button>
    <button v-on:click="Subtract(10)">Subtract </button>
    <button v-on:click="age=0" >Reset </button> 
    <p> {{ age }} năm thành lập </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    age: Number
  },
  value : {
    characters: ['jone','ád','áda']
  },
  methods:{
    Add: function (inc){
      let number_age = Number(this.age);
      number_age+=inc;
      this.age = number_age; 
      console.log (this.age); 
    },
    Subtract: function (dec){
      if (this.age > 0){
        if (this.age-dec < 0){
           this.age = 0;
          } else this.age-=dec;
      } else this.age = 0;   
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
