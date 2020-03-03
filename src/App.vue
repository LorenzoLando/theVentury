<template>
  <div>
    <body>
      <!-- <app-header></app-header> -->
      <app-header2></app-header2>
      <app-about></app-about>
      <app-careers></app-careers>
      <app-footer></app-footer>
    </body>
  </div>
</template>

<script>
import Header from './componets/header.vue'
import Header2 from './componets/header2.vue'
import Careers from './componets/careers.vue'
import About from './componets/about.vue'
import Footer from './componets/footer.vue'
export default {
  components: {
    'app-header': Header,
    'app-header2': Header2,
    'app-careers': Careers,
    'app-about': About,
    'app-footer': Footer

  },
  data () {
    return {
      counter: true
    }
  },
  mounted:{

  },
  methods:{
    
  }
}
</script>

<style lang="scss">

html {
  scroll-behavior: smooth;
}
body {
  // background-color:  #adadad;
}
</style>





