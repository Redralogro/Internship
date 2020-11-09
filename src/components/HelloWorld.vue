<template>
  <div class="hello">
    <header>
        <nav>
            <div class="row">
            
                <ul class="main-nav js--main-nav">
                    <li v-for="nav in nav_element" :key="nav.name"><a v-bind:href="nav.name">{{nav.label}} </a></li>
                </ul>
                <a class="mobile-nav-icon js--nav-icon"><i
                            class="ion-navicon-round"></i></a>
            </div>
        </nav>
        <div class="hero-text-box">
            <h1>
                Goodbye junk food.<br> Hello super healthy meals.
            </h1>
            <a href="#" class="btn btn-full js--scroll-to-plans">I’m hungry
                </a>
            <a href="#" class="btn btn-ghost js--scroll-to-start">Show me
                    more</a>
        </div>
    </header>
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
