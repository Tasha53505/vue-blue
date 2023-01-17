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

<div class="bgImg container">
  <h2>Tech Support Brought to you by</h2>
  <h1 class="brandTitle">Brand name Here</h1>
  <img src="src/assets/images/HomeImgTech.svg" alt="img" class="homeImg">
  <hr>
  <h4 class="slogan">Slogan  Lorem ipsum dolor sit amet consectetur adipisicing elit</h4>

  <button class="learnBtn" id="learnMore">Learn more</button>  
  <button class="galleryBtn">Gallery </button>  
 
</div>
<!-- After blue content - Meet tht team
<div  class="meetContainerRow">
  <div class="meetRowColumn">
      <h4 class="columnOne">Slogan Lorem ipsum dolor sit, amet consectetur adipisicing elit. </h4>
      <h1 class="meetTitle">More than 5000000 companies want a website from us</h1>
  </div>
</div> -->



<!-- testing HTML -->
<div class="parent">
  <div class="child">
    <h4 class="columnOne">Slogan Lorem ipsum dolor sit, amet consectetur adipisicing elit. </h4>
    <h1 class="meetTitle">More than 5000000 companies want a website from us</h1>
  </div>

  <div class="child2">
    <h2>This is the right</h2>
    <img src="src/assets/images/femaleAvatar.svg" alt="femaleAvatar" class="femaleAvatar">
  </div>

</div>

<!-- -------------------------- -->

</main>
</template>

<style scoped>
/* Testing CSS  */
.parent {
  display: flex;
  flex-direction: row;
}

.child {
  width: 100%;
  height: 30vh;
  /* background-color: rgb(214, 245, 255); */
  text-align: left;
  color: black;
  padding-left: 1rem;

}

.child2 {
  width: 100%;
  height: 30vh;
  background-color: rgb(173, 236, 255);
  text-align: center;

}

/* ----------- Images ------------ */
.femaleAvatar {
  width: 15%;
}

.homeImg {
float: right;
/* display: flex;
flex-direction: column;
margin: auto; */
width: 30rem;
position: relative;
top: -8rem;

}

/* ------------------------- */
h2, h1  {
  padding: 1rem;
  color: white;
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;

}

.brandTitle {
  margin-top: -25px;
}

.invisible {
    text-indent: 110%;
    white-space: nowrap;
    overflow: hidden;
}

.bgImg {
  background-image: url("src/assets/images/backgroundTransparent.png");
  width: 100%;
  height: 52vh;
}

.slogan {
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  font-size: large;
  color: white;
  margin-top: 0.5em;

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



.container {

}

.flexItem {

}
/* ------ Buttons --------  */
button {
  margin-left: 1rem;
  margin-top: 1rem;
  cursor: pointer;

}

.learnBtn {
  padding: 0.5em;
  background-color: white;
  border: white solid 4px;
  border-radius: 15px;
  text-align: center;
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  font-size: 16px;
}

.learnBtn:hover {
  border-radius: 15px;
  transition: 0.4;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 5px 8px;
}

.galleryBtn {
  padding: 0.5em;
  background-color: transparent;
  border: none;
  font-size: 15px;
  color: white;
}
/* Meeet the team  */
.meetContainerRow {
  padding: 1rem;
  display: flex;
  flex-direction: row;
  align-items: flex-start;

}

.meetTitle {
  color: black;
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  width: 60%;
  font-size: 35px;
  
}




@media (max-width: 1024px) {
.bgImg {
  background-image: url("src/assets/images/backgroundTransparentMedia.png");
  width: 100%;
  height: 80vh;
}

.homeImg {
/* display: flex;
flex-direction: column;
margin: auto; */

}

h2 {
  /* font-size: 1px; */
}


}
</style>
