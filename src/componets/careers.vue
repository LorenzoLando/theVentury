<template>
  <div id="careers" class="container">
            <div class="row mb-2">
              <div class="col-md-6" v-for="(job, index) in jobs" v-bind:key="index">
                <div class="card flex-md-row mb-4 shadow-sm h-md-250">
                  <div class="card-body d-flex flex-column align-items-start">
                    <strong class="d-inline-block mb-2 text-primary"></strong>
                    <h3 class="mb-0">
                      <a class="" href="#">{{job.title}}</a>
                    </h3>
                    <div class="mb-1 text-muted">{{job.location}}</div>
                    <p class="card-text mb-auto">{{job.description}}</p>
                    <div class="checkbox" v-for="(skill, index) in job.skills" v-bind:key="index">
                      <label><input type="checkbox" value="" checked>{{skill}}</label>
                    </div>
                    <a href="#">Continue reading</a>
                  </div>
                  <img class="card-img-right flex-auto d-none d-lg-block" data-src="holder.js/200x250?theme=thumb" alt="Thumbnail [200x250]" style="width: 200px; height: 250px;" v-bind:src="job.img" data-holder-rendered="true">
                </div>
              </div>
            </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
      jobs: [
        {
          title: "Front-end Developer",
          location: 'New York',
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Eu ultrices vitae auctor eu augue ut lectus arcu. Sit amet commodo nulla facilisi. Cursus mattis molestie a iaculis. Senectus et netus et malesuada. Arcu non odio euismod lacinia at quis risus sed vulputate. Viverra nam libero justo laoreet sit amet cursus sit. Et sollicitudin ac orci phasellus egestas tellus rutrum tellus. Odio eu feugiat pretium nibh ipsum consequat nisl vel. Aliquet sagittis id consectetur purus ut faucibus pulvinar elementum integer.",
          img: 'src/assets/images/front.jpg',
          skills: ['Javascript', 'CSS', 'Vue.js']
        },
         {
          title: "Back-end Developer",
          location: 'Wien',
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Eu ultrices vitae auctor eu augue ut lectus arcu. Sit amet commodo nulla facilisi. Cursus mattis molestie a iaculis. Senectus et netus et malesuada. Arcu non odio euismod lacinia at quis risus sed vulputate. Viverra nam libero justo laoreet sit amet cursus sit. Et sollicitudin ac orci phasellus egestas tellus rutrum tellus. Odio eu feugiat pretium nibh ipsum consequat nisl vel. Aliquet sagittis id consectetur purus ut faucibus pulvinar elementum integer.",
          img: 'src/assets/images/back.jpg',
          skills: ['Python','Node.js','SQL']
        }
      ]
    }
  } 
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
@import url('https://fonts.googleapis.com/css?family=Oswald&display=swap');
$text-color: #8b3e6e;
.card {
  
  border-radius: 10%;
  -webkit-box-shadow: -4px 14px 5px -8px rgba(0,0,0,0.75);
  -moz-box-shadow: -4px 14px 5px -8px rgba(0,0,0,0.75);
  box-shadow: -4px 14px 5px -8px rgba(0,0,0,0.75);
  background-color: #f8f9fa;
  margin: 1rem;
  color: $text-color;
}


.card-text {
  width: 250px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.card img {
  //height: 60%;
  border-radius: 0 10% 10% 0;
 
}

a {
  text-decoration: none;
  color: $text-color;
}


</style>
