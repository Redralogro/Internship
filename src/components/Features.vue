<template>
  <section class="section-features js--section-features" id="features">
        <div class="row js--wp-1">
            <h2>Get food fast &mdash; not fast food.</h2>
            <p class="long-copy">
                Hello, we’re Omnifood, your new premium food delivery service. We know you’re always busy. No time for cooking. So let us take care of that, we’re really good at it, we promise!
            </p>
            
            <div class="row ">
                 <div class="col span-1-of-4 box" v-for="feature in features" :key="feature.name">
                    <i v-bind:class="feature.name"></i>
                    <h3>

                        {{feature.title}}

                    </h3>
                    <p>
                        {{feature.description}}
                    </p>
                </div>
            </div>
        </div>

    </section>
</template>

<script>
export default {
  name: 'Features',
  data() {
        return {
           features: [
               {
                  name:'ion-ios-infinite-outline icon-big',
                  title:'Up to 365 days/year',
                  description:"Never cook again! We really mean that. Our subscription plans include up to 365 days/year coverage. You can also choose to order more flexibly if that's your style."
              },
               {
                  name:'ion-ios-stopwatch-outline icon-big',
                  title:'Ready in 20 minutes',
                  description:"You're only twenty minutes away from your delicious and super healthy meals delivered right to your home. We work with the best chefs in each town to ensure that you're 100% happy."
                },
              {
                  name:'ion-ios-nutrition-outline icon-big',
                  title:'100% organic',
                  description:"All our vegetables are fresh, organic and local. Animals are raised without added hormones or antibiotics. Good for your health, the environment, and it also tastes better!"
                },
              {
                  name:'ion-ios-cart-outline icon-big',
                  title:'Order anything',
                  description:"We don't limit your creativity, which means you can order whatever you feel like. You can also choose from our menu containing over 100 delicious meals. It's up to you!"
                }
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
