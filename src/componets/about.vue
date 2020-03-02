<template>
  <div id="about" class="container">
	  <div class="row">
		   <div class="col-lg"> 
			   <!--Google map-->
				<div id="map-container-google-1" class="z-depth-1-half map-container" style="height: 700px">
				<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d10635.589166698264!2d16.36582019407425!3d48.20859421754286!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x476d079f7175de6b%3A0xe07936082ee4ec40!2sStephansdom%2C%201010%20Vienna%2C%20Austria!5e0!3m2!1sen!2sro!4v1569322893839!5m2!1sen!2sro"
					title="companyAddress" frameborder="0"></iframe>
				</div>
			</div>
			<div class="col-lg">
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
	  companyDescription : "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Et malesuada fames ac turpis egestas maecenas pharetra. Commodo quis imperdiet massa tincidunt nunc. Elementum pulvinar etiam non quam lacus suspendisse faucibus interdum posuere. Arcu dui vivamus arcu felis. Lacus sed turpis tincidunt id aliquet risus. Placerat duis ultricies lacus sed turpis. Egestas fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien. Ultricies integer quis auctor elit sed vulputate mi sit amet. Tellus in metus vulputate eu. Nunc eget lorem dolor sed. Augue lacus viverra vitae congue eu. Sem viverra aliquet eget sit amet tellus cras adipiscing. Feugiat in fermentum posuere urna."
	}
	}
}
</script>

<style lang="scss" scoped>
$text-color: #8b3e6e;

#map-container-google-1 {
	
}
section {
	color: $text-color;
	padding: 5rem;
	text-align: justify;
}

section h2 {
	text-align: center;
	margin-bottom: 3rem;
}
iframe {
	height: 100%;
	width: 100%;
	padding: 5rem;
	border-radius: 25%;
}

h2 {
	text-decoration: underline;
}
</style>
