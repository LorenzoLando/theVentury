<template>
  <div>
    <body>
      <app-header></app-header>
      <app-careers></app-careers>
      <app-about></app-about>
      <app-footer></app-footer>
    </body>
  </div>
</template>

<script>
import Header from './componets/header.vue'
import Careers from './componets/careers.vue'
import About from './componets/about.vue'
import Footer from './componets/footer.vue'
export default {
  components: {
    'app-header': Header,
    'app-careers': Careers,
    'app-about': About,
    'app-footer': Footer

  },
  data () {
    return {
      counter: true
    }
  },
  methods:{
    
  }
}
</script>

<style lang="scss">

html {
  scroll-behavior: smooth;
}
</style>





