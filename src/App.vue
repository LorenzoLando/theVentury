<template>
  <div>
    <app-header></app-header>
    <app-body></app-body>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './componets/header.vue'
import Body from './componets/body.vue'
import Footer from './componets/footer.vue'
export default {
  components: {
    'app-header': Header,
    'app-body': Body,
    'app-footer': Footer

  },
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
