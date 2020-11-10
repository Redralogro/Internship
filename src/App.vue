<template>
  <div id="app">
  <header>
    <Nav/>
    <textBox/>
  </header>
  <Features/>
  <Meals/>
  <Steps/>
  </div>
</template>

<script>
import Nav from './components/header/Nav.vue'
import textBox from './components/header/Text-box.vue'
import Features from './components/Features.vue'
import Meals from './components/Meals.vue'
import Steps from './components/Steps.vue'
export default {
  name: 'App',
  components: {
    Nav,
    textBox,
    Features, 
    Meals, Steps
  }
}
</script>

<style>

</style>
