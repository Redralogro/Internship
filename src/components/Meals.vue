<template>
  <section class="section-meals">
        <ul class="meals-showcase clearfix">
           <li>
                <figure class="meal-photo">
                    <img src="../assets/img/1.jpg" alt="Korean bibimbap
                            with egg and vegetables">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/2.jpg" alt="Simple italian
                            pizza with cherry tomatoes">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/3.jpg" alt="Chicken breast
                            steak with vegetables">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/4.jpg" alt="Autumn pumpkin
                            soup">
                </figure>
            </li>

        </ul>
        <ul class="meals-showcase clearfix">
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/5.jpg" alt="Paleo beef steak
                            with vegetables">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/6.jpg" alt="Healthy baguette
                            with egg and vegetables">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/7.jpg" alt="Burger with
                            cheddar and bacon">
                </figure>
            </li>
            <li>
                <figure class="meal-photo">
                    <img src="../assets/img/8.jpg" alt="Granola with
                            cherries and strawberries">
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
                {image:'../assets/img/1.jpg',alt:'Korean bibimbap with egg and vegetables'},
                {image:'../assets/img/2.jpg',alt:'Simple italian pizza with cherry tomatoes'},
                {image:'../assets/img/3.jpg',alt:'Chicken breast steak with vegetables'},
                {image:'../assets/img/4.jpg',alt:'Autumn pumpkin soup'},
            ],
            showcases2:[
                {src:'../assets/img/5.jpg',alt:'Paleo beef steak with vegetables'},
                {src:'../assets/img/6.jpg',alt:'Healthy baguette with egg and vegetables'},
                {src:'../assets/img/7.jpg',alt:'Burger with cheddar and bacon'},
                {src:'../assets/img/8.jpg',alt:'Granola with cherries and strawberries'},
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
