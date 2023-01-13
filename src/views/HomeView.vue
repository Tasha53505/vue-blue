<script setup>
</script>

<template>
  <main>
  <!-- Div for image
NavBAr
Header
image float right
Hr line
h4
2 buttons -->

<div class="bgImg">
  <h2>Tech Support Brought to you by</h2>
  <h1>Brand name Here</h1>
  <img src="src/assets/images/techSupport.png" alt="img" class="homeImg">
  <hr>
  <h4>Slogan  Lorem ipsum dolor sit amet consectetur adipisicing elit</h4>
  <button>Button 1</button>  
  <button>Button 2</button>  






  
</div>


</main>
</template>

<style scoped>
h2, h1  {
  padding: 1rem;
  color: white;
}

.invisible {
    text-indent: 110%;
    white-space: nowrap;
    overflow: hidden;
}

.bgImg {
  background-image: url("src/assets/images/backgroundTransparent.png");
  width: 100%;
  height: 100%;
}
hr {
  width: 15%;
  border: none;
  height: 4px;
  background: white;
  margin-left: 1rem;

  /*   position: relative;
        top: 20px;
        border: none;
        height: 12px;
        background: black;
        margin-bottom: 50px; */
}


h4 {
  margin-left: 1rem;

}
h1 {
  font-weight: 600;
  font-size: 42px;
}

.homeImg {
float: right;
/* display: flex;
flex-direction: column;
margin: auto; */
width: 50%;

}
</style>
