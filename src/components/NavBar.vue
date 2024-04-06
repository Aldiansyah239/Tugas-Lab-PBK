<template>
  <header class="header">
   <nav class="navigation">
     <a href="#home">Home</a>
     <a href="#profile">Profile</a>
     <a href="#portfolio">Portfolio</a>
     <a href="#gallery">Gallery</a>
     <a href="#achievement">Achievement</a>
   </nav>
   <a href="#" class="more-link"></a>
 </header>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.header {
  background-color: #212c3d;
  padding: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.navigation {
  display: flex;
  justify-content: center;
  align-items: center;
}

.navigation a {
  color: #fff;
  text-decoration: none;
  margin-right: 20px;
}

.navigation a:hover {
  color: #c06014;
  font-size: 1.1em; /* slightly bigger */
}

</style>
