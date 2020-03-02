<template>
    <div>
      <header>
       <nav id="#about" class="navbar navbar-expand-lg navbar-light bg-light">
                <a class="navbar-brand" href="#"><!-- navbar brand -->
                    <img class="navbar-brand dark-logo lazy loaded" src="https://theventury.com/wp-content/uploads/2019/12/logo_small.png" data-src="https://theventury.com/wp-content/uploads/2019/12/logo_small.png" data-rjs="https://theventury.com/wp-content/uploads/2019/12/logo_big.png" alt="TheVentury" data-was-processed="true">
                    <!-- /navbar brand --></a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                  <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                  <ul class="navbar-nav">
                    <li class="nav-item active" v-for="(navbarLink, index) in navbarLinks" v-bind:key="index">
                      <a class="nav-link" v-bind:href="navbarLink.link">{{navbarLink.linkTitle}}</a>
                    </li>
                  </ul>
                </div>
              </nav>
      </header>
    </div>
</template>
<script>

export default {
  data () {
    return {
      navbarLinks: [{linkTitle: 'About Us', link: '#about'},{linkTitle: 'Careers',link: '#careers'},{linkTitle: 'Contacts',link: '#footer'}]
    }
  },
  methods: {

  },
  mounted(){
     
    }
}
</script>

<style lang="scss" scoped>
   @import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
   @import url('https://fonts.googleapis.com/css?family=Oswald&display=swap');
   $text-color: #8b3e6e;
   
   
   .navbar-brand {
        height: 5rem;
        width: 12rem;
        margin-left: 3rem;
    }

    .navbar-toggler {
        border-color: $text-color; 
    }

    #navbarNav {
      justify-content: flex-end;
    }
   
   header > nav {
        
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        color: $text-color;
    }

    header > nav div:last-child {
        margin-left: 5rem;
        width: 60%;
        
    }

    ul{
          display: flex;
          flex-direction: row;
          justify-content: space-around;
          margin-right: 8rem;
    }
    
    ul > li {
        padding-left: 5rem;
    }

    ul > li  > a {
         
            color: $text-color !important;
            font-family: Oswald,Arial,sans-serif;
            font-weight: 500;
            text-transform: uppercase;
            font-size: 14px;
            font-variant-ligatures:none;
            font-weight:500;
            letter-spacing:2px;
            list-style-type:none;
            text-shadow:rgba(0, 0, 0, 0.01) 0px 0px 1px;
            text-size-adjust:100%;
      }

      .nav-link {
        text-decoration: underline;
      } 
    
</style>
