<template>
<Nav />
<div class="bg-[#141516]">
<Hero />
</div>
<Feature />
<div class="bg-[#141516] overflow-hidden">
<Help />
</div>
<Famous />
<Footer />
</template>

<script>
import Nav from './components/Nav.vue'
import Feature from './views/Feature.vue'
import Help from './views/Help.vue'
import Hero from './views/Hero.vue'
import AOS from 'aos'
import Footer from './components/Footer.vue'
import Famous from './views/Famous.vue'
export default {
  components: { Nav, Hero, Feature, Help, Footer, Famous },
  name: 'App',
  mounted() {
    AOS.init({})
  },
}
</script>
