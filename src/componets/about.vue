<template>
  <div class="container">
	  <div class="row">
		   <div class="col-sm">
			   <!--Google map-->
				<div id="map-container-google-1" class="z-depth-1-half map-container" style="height: 500px">
				<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d10635.589166698264!2d16.36582019407425!3d48.20859421754286!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x476d079f7175de6b%3A0xe07936082ee4ec40!2sStephansdom%2C%201010%20Vienna%2C%20Austria!5e0!3m2!1sen!2sro!4v1569322893839!5m2!1sen!2sro"
					title="companyAddress" frameborder="0"></iframe>
				</div>
			</div>
			<div class="col-sm">
				<section>
					<h2>About Us</h2>
						<p>{{companyDescription}}</p>
				</section>
			</div>
		</div>
</div>
</template>

<script>
 export default {
 data () {
    return {
	  companyDescription : "At TheVentury, we are passionate about innovation, technology and the positive change these can create. We bring brilliant minds together 						to provide lean & hands-on services in innovation management, data & software engineering and growth marketing to startups and corporates 						along the whole journey from idea generation to global impact."
	}
	}
}
</script>

<style lang="scss" scoped>
$text-color: #8b3e6e;

// .container {
// 	background-color: red;
// 	width: 100%;
// }

section {
	color: $text-color;
	padding: 5rem;
	text-align: justify;
}

section h2 {
	text-align: center;
	margin-bottom: 2rem;
}
iframe {
	height: 100%;
	width: 100%;
	padding: 5rem;
}
</style>
