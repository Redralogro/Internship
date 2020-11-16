<template>
  <section class="section-meals">
        <ul class="meals-showcase clearfix">     
           <li v-for="showcase in showcases1" :key="showcase.image">
                <figure class="meal-photo">
                    <img :src="`/img/${showcase.image}.jpg`" :alt="showcase.alt">
                </figure>
            </li>
        </ul>
        <ul class="meals-showcase clearfix">
            <li v-for="showcases in showcases2" :key="showcases.image">
                <figure class="meal-photo">
                    <img :src="`/img/${showcases.image}.jpg`" :alt="showcases.alt">
                </figure>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
        return {
            showcases1:[
                {image:'1',alt:'Korean bibimbap with egg and vegetables'},
                {image:'2',alt:'Simple italian pizza with cherry tomatoes'},
                {image:'3',alt:'Chicken breast steak with vegetables'},
                {image:'4',alt:'Autumn pumpkin soup'},
            ],
            showcases2:[
                {image:'5',alt:'Paleo beef steak with vegetables'},
                {image:'6',alt:'Healthy baguette with egg and vegetables'},
                {image:'7',alt:'Burger with cheddar and bacon'},
                {image:'8',alt:'Granola with cherries and strawberries'},
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
