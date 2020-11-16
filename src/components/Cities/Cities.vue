<template>
    <div class="col span-1-of-4 box">
                    <img :src="`/img/${img}.jpg`" alt="Cities">
                    <h3>{{city}}</h3>
                    <div class="city-feature">
                        <i class="ion-ios-person icon-small"></i> {{eaters}}
                    </div>
                    <div class="city-feature">
                        <i class="ion-ios-star icon-small"></i> {{chefs}}
                    </div>
                    <div class="city-feature">
                        <i class="ion-social-twitter icon-small"></i>
                        <a href="#">{{twitter}}</a>
                    </div>
                </div>
</template>

<script>
export default {
    name: 'Cities',
  props :{
   city: String,
   eaters : String,
   chefs : String,
   twitter : String,
   alt : String,
   img : String,
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
