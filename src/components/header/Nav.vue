<template>
  <div class="hello">
    
        <nav>
            <div class="row">
            <img src="../../assets/img/logo-white.png" alt="Omnifood
                        logo" class="logo">
            <img src="../../assets/img/logo.png" alt="Omnifood logo" class="logo-black">
                <ul class="main-nav js--main-nav">
                    <li v-for="nav in nav_element" :key="nav.name"><a v-bind:href="nav.name">{{nav.label}} </a></li>
                </ul>
                <a class="mobile-nav-icon js--nav-icon"><i
                            class="ion-navicon-round"></i></a>
            </div>
        </nav>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
        return {
            nav_element: [
              {name:'#features',label:'Food delivery'},
              {name:'#works',label:'How it works'},
              {name:'#cities',label:'Our cities'},
              {name:'#plans',label:'Sign up'}
             ]
        };
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

</style>
