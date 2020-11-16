<template>
  <section class="section-cities" id="cities">
        <div class="row js--wp-3">
            <h2>
                We're currently in these cities
            </h2>
            <div class="row">
            <div class="js--wp-3" v-for="info in infoCity" :key="info.img">
               <Cities v-bind:img="info.img" v-bind:city="info.city" v-bind:eaters="info.eaters" v-bind:chefs="info.chefs" v-bind:twitter="info.twitter"/>
            </div>
            </div>
        </div>
    </section>
</template>

<script>
import Cities from './Cities/Cities.vue'
export default {
  name: 'HelloWorld',
  components: {
      Cities
  },
  data() {
        return {
            infoCity:[
              {img:'lisbon-3',city:'Lisbon',eaters:'1600+ happy eaters',chefs:'60+ top chefs',twitter:'@omnifood_lx'},
              {img:'san-francisco',city:'San Francisco',eaters:'3700+ happy eaters',chefs:'160+ top chefs',twitter:'@omnifood_sf'},
              {img:'berlin',city:'Berlin',eaters:'2300+ happy eaters',chefs:'110+ top chefs',twitter:'@omnifood_berlin'},
              {img:'london',city:'London',eaters:'1200+ happy eaters',chefs:'50+ top chefs',twitter:'@omnifood_london'}     
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

</style>
