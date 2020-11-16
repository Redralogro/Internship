<template>
  <div id="app">
  <header>
    <Nav/>
    <textBox/>
  </header>
  <Features/>
  <Meals/>
  <Steps/>
  <SectionCities/>
  <SectionTestimonials/>
  <SectionPlans/>
  <SectionForm/>
  <Footer/>
  </div>
</template>

<script>
import Nav from './components/header/Nav.vue'
import textBox from './components/header/Text-box.vue'
import Features from './components/Features.vue'
import Meals from './components/Meals.vue'
import Steps from './components/Steps.vue'
import SectionCities from './components/Section_Cities.vue'
import SectionTestimonials from './components/Section_testimonials.vue'
import SectionPlans from './components/Section_plans.vue'
import SectionForm from './components/Section_form.vue'
import Footer from './components/footer.vue'
export default {
  name: 'App',
  components: {
    Nav,textBox,Features, 
    Meals, Steps,
    SectionCities,
    SectionTestimonials,
    SectionPlans,SectionForm,Footer
  }
}
</script>

<style>

</style>
