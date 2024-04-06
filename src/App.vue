<template>
  <div id="app">
    <NavBar />
    
    <section class="home" id="home">
  <div class="content">
    <div class="text">
      <h2>Hi, Im A Student of Riau Islamic University</h2>
      <p>“Two things are infinite: the universe and human stupidity;<br>and I'm not sure about the universe.”<br>― Albert Einstein</p>
    </div>

 </div>

    <div class="image">
      <img src="img/aldiansyah1.jpg" alt="Profile Image">
    </div>
 
</section>

    
    <section class="profile" id="profile">
      
      <h2>Profile</h2>

    <div class="Profile_content">


      <h2>Data Diri</h2>
      <h1>Aldiansyah</h1>
      <p>Pekanbaru, 4 Januari 2004</p>


      <h2>Pendidikan</h2>
      <ul>
        <li>SDN 001 Pekanbaru</li>
        <li>SMPN 7 Pekanbaru</li>
        <li>SMAN 6 Pekanbaru</li>
        <li>Universitas Islam Riau</li>
      </ul>
    </div>

    <h2>Hobi</h2>
      <p>Futsal</p>
      <p>Renang</p>
    </section>
    

      
      <section class="Portfolio" id="portfolio">
      <h2 class="heading">Portofolio</h2>
      <div class="portfolio">

         <div class="portfolio1">
                <a target= "-blank"><img src="img/Projek1.jpg" alt="Projek 1"> </a>     
                <h2>marut</h2>
              
            </div>
          </div>

    </section>

    <section class="Gallery" id="gallery">
  <h2 class="heading">Gallery</h2>
  <div class="gallery-images">
    <div class="gallery-item">
      <img src="img/aldiansyah1.jpg" alt="Gambar 1">
    </div>
    <div class="gallery-item">
      <img src="img/aldiansyah2.jpg" alt="Gambar 2">
    </div>
    <div class="gallery-item">
      <img src="img/aldiansyah3.jpg" alt="Gambar 3">
    </div>
    <div class="gallery-item">
      <img src="img/aldiansyah4.jpg" alt="Gambar 4">
    </div>
  </div>
</section>

    
    <section class="achievement" id="achievement">
      <!-- Achievement content goes here -->
      <h2>Achievement</h2>
      <p>Discover our achievements in this section.</p>
    </section>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
  }
}
</script>

<style>

body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #566357; /* Set your desired background color here */
}


.header {
    position: fixed;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    padding: 20px 10%;
    background: transparent;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 100;
}

section {
  padding: 50px 20px;
  color: #fff;
  text-align: center;
}

/* Background colors for each section */
.home {
  min-height: 100vh;
  background-color: #39424e;
  display: flex;
  justify-content: center; /* Center the content horizontally */
  align-items: center; /* Center the content vertically */
}

.content {
  display: flex; /* Use flexbox for layout */
  flex-direction: row; /* Align items horizontally */
}

.text {
  flex: 1; /* Take remaining space */
  text-align: left; /* Align text to the left */
}

.image {
  margin-left: 20px; /* Add space between text and image */
}

.image img {
  max-width: 40%; 
  border: 2px solid #fff; /* Add a white border around the image */
  border-radius: 5px;/* Ensure image doesn't exceed container */
}


.text h2 {
  font-size: 3.3em;
  margin: 0 0 20px 0; 
}


.text p {
  font-size: 2em;
  margin: 0 0 20px 0; /* Add bottom margin */
}


.profile {
  min-height: 100vh;
  background-color: #3e4a5a;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.profile h2 {
   color: #c06014;
}


.Profile_content {
  margin-top: 20px;
}

.Profile_content h2 {
  font-size: 1.5em;
  margin-bottom: 10px;
}

.Profile_content ul {
  list-style: none;
  padding: 0;
}

.Profile_content li {
  font-size: 1.2em;
  margin-bottom: 5px;
}



.heading {
  font-size: 2rem;
  margin-bottom: 1rem;
  text-align: center;
  color: #fff; 
}


.Portfolio {
  min-height: 100vh; 
  padding: 75px 50px;
  background: #435366;
}

.heading {
  font-size: 2rem;
  margin-bottom: 1rem;
  text-align: center;
  color: #fff;
}

.portfolio {
  display: flex;
  grid-template-columns: repeat(2, minmax(auto-fit, 1fr));
  gap: 20px;
}


.portfolio1 {
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: hidden;
  cursor: pointer;
  padding: 20px; 
  color: #fff; 
  text-align: center; 
  border: 5px solid #fff; 
  box-sizing: border-box;
}

.portfolio1 img {
  width: 250px;
  transition: transform 0.3s;
}

.portfolio1 p {
    text-align: left;
}
.portfolio1 :hover img {
  transform: scale(1.1);
}




  .heading {
    font-size: 2rem;
    margin-bottom: 1rem;
    text-align: center;
    color:#c06014; 
  }
  .Gallery {
  background-color: #485a73;
  min-height: 100vh;
  padding: 75px 50px;
  text-align: center; /* Center the heading and images */
}

.heading {
  font-size: 2rem;
  margin-bottom: 1rem;
  color: #c06014;
}

.gallery-images {
  display: flex;
  flex-wrap: wrap; /* Allow items to wrap to the next line */
  justify-content: center;
}

.gallery-item {
  margin: 10px; /* Add some space between each gallery item */
}

.gallery-item img {
  width: 350px;
  transition: transform 0.3s;
  max-width: 100%; /* Ensure images fill their container */
  border: 2px solid #fff;
  border-radius: 5px;
}




.achievement {
  min-height: 100vh;
  background-color: #4d627f;
}

.achievement h2 {
   color: #c06014;
}

/* Heading styles */
h2 {
  font-size: 2em;
  margin-bottom: 20px;
}

p {
  font-size: 1.2em;
}


</style>
