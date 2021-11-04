<template>
  <div id="App">
    <router-view/>
  </div>
</template>

<script>
export default {
  
}
</script>

<style>
:root {
  --white: #ffffff;
  --gray: #999999;
  --purple: #442c61;
  --yellow: #f79e1b;
  --red: #eb001b;
  --light-blue: #0061ff;
  --dark-blue: #08189e;
  --dark-gray: #121212
}
*,
*::before,
*::after{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Poppins, sans-serif;
}
</style>
