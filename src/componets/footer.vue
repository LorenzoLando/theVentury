<template>
  <div>
    <img class="lazy loaded" id="footer-astronaut" src="https://theventury.com/wp-content/uploads/2019/11/footer_1920.png" data-src="https://theventury.com/wp-content/uploads/2019/11/footer_1920.png" data-was-processed="true">
   <!-- Footer -->
    <footer id="footer" class="page-footer font-small mdb-color lighten-3 pt-4">
  <!-- Footer Links -->
      <div class="container text-center text-md-left">
      <!-- Grid row -->
        <div class="row">
<!-- Grid column -->
          <div class="col-md-4 col-lg-3 mr-auto my-md-4 my-0 mt-4 mb-1">
            <!-- Content -->
            <h5 class="font-weight-bold text-uppercase mb-4">THEVENTURY GMBH</h5>
            <p>Praterstrasse 1 / Space 38</p>
            <p>1020 Vienna, Austria</p>
          </div>
          <!-- Grid column -->
          <hr class="clearfix w-100 d-md-none">
          <!-- Grid column -->
          <div class="col-md-2 col-lg-2 mx-auto my-md-4 my-0 mt-4 mb-1">
        <!-- Links -->
        <h5 class="font-weight-bold text-uppercase mb-4">About</h5>

            <ul class="list-unstyled">

              <li v-for="(footerLink, index) in footerLinks" v-bind:key="index">
                  <p>
                      <a v-bind:href="footerLink.link">{{footerLink.linkTitle}}</a>
                  </p>
              </li>
            </ul>

          </div>
          <!-- Grid column -->

          <hr class="clearfix w-100 d-md-none">

          <!-- Grid column -->
         

        
          <div class="col-md-4 col-lg-3 mx-auto my-md-4 my-0 mt-4 mb-1">
              <a href="https://theventury.com"><img width="182" height="273" src="https://theventury.com/wp-content/uploads/2019/10/Logo_Basic_Sm.png" data-src="https://theventury.com/wp-content/uploads/2019/10/Logo_Basic_Sm.png" class="image wp-image-62125 attachment-full size-full lazy loaded" alt="" style="max-width: 100%; height: auto;" data-was-processed="true"></a>
         </div>
          <!-- Grid column -->

          <hr class="clearfix w-100 d-md-none">
          <!-- end trial -->

          <!-- Grid column -->
          <div class="col-md-2 col-lg-2 text-center mx-auto my-4">

            <!-- Social buttons -->
            <h5 class="font-weight-bold text-uppercase mb-4">Follow Us</h5>

            <!-- Facebook -->
            <a type="button" class="btn-floating btn-fb">
              <img src="src/assets/images/facebook.png">
              
            </a>
            <!-- Twitter -->
            <a type="button" class="btn-floating btn-tw">
              <img src="src/assets/images/twitter.png">
            </a>
            <!-- Google +-->
            <a type="button" class="btn-floating btn-gplus">
              <img src="src/assets/images/instagram.png">
            </a>
            <!-- Dribbble -->
            <a type="button" class="btn-floating btn-dribbble">
             <img src="src/assets/images/twitch.png">
            </a>

          </div>
          <!-- Grid column -->

        </div>
        <!-- Grid row -->

      </div>
      <!-- Footer Links -->

      <!-- Copyright -->
      <div class="footer-copyright text-center py-3">© 2020 Copyright:
        <a href="https://lorenzolando.github.io/Portfolio/">Lorenzo Lando</a>
      </div>
      <!-- Copyright -->

</footer>
<!-- Footer -->
  </div>
</template>

<script>
export default {
  data () {
    return {
      footerLinks: [{linkTitle: 'About Us', link: '#about'},{linkTitle: 'Careers',link: '#careers'},{linkTitle: 'Contacts',link: '#footer'}]
    }
  }
}
</script>

<style lang="scss" scoped>

$main-color: #333333;
#footer-astronaut {
  max-width: 100%;
}

footer {
  background-color:  $main-color;
  color: white;
}

a {
  color: white;
}

.btn-floating > img {
  height: 4rem;
  width: 4rem;
  margin: 5px;
} 

</style>
