<template>
  <div id="app">
      <main>
        <div class="search-box">
          <input 
            type="text" 
            class="search-bar" 
            placeholder="Search..."    
          />
        </div>
        <div class="weather-wrap">
          <div class="location-box">
            <p class="location">Tours, FR</p>
            <p class="date">Mercredi 23 Février 2022</p>
          </div>
          <div class="weather-box">
            <div class="temp">9°C</div>
            <div class="weather">Pluie</div>
          </div>
        </div>
      </main>
   
  </div>
</template>

<script>

export default {
  name:'app',
  data () {
    return {
      api_key:'45702f39f87a2a68162f4f09571b46f0'
    }
  }
  
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'montserrat', sans-serif;
}
#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: bottom;
  transition: 0.4s;
}

main{
  min-height: 100vh;
  padding: 25px;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.20), rgba(0, 0, 0, 0.60));
}

.search-box{
  width: 100%;
  margin-bottom: 30px;
}

.search-box .search-bar {
  display: block;
  width: 100%;
  padding: 15px;

  color: #303030;
  font-size: 20px;

  appearance: none;
  border: none;
  outline: none;
  background: none;

  box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.25);
  background-color: rgba(260, 260, 260, 0.8);
  border-radius: 0px 16px 0px 16px;
  transition: 0.4s;
}

.search-box .search-bar:focus {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 16px 0px 16px 0px;
}



</style>
