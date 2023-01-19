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





<!-- testing HTML -->
<div class="parent">
  <div class="child">
    <h4 class="columnOne">Slogan Lorem ipsum dolor sit, amet consectetur adipisicing elit. </h4>
    <h1 class="meetTitle">More than 5000000 companies want a website from us</h1>
    <button class="madeBtn">What We've Made</button>
  </div>

  <div class="child2">
    <!-- <h2>This is the right</h2> -->
    <div class="cardContainer">
      <img src="src/assets/images/femaleAvatar.svg" alt="femaleAvatar" class="femaleAvatar">
      <h3 class="cardName">Bold Name</h3>

      <a href="about">
      <img src="src/assets/images/arrow.svg" alt="arrow" class="arrowImg">
    </a>
    </div>
    <p class="cardText">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat, ipsam alias quas consequuntur aliquam corrupti temporibus incidunt veritatis! Eos tempora nisi officia corrupti dolores ut.</p>

  </div>

  
  

</div>

<!-- -------------------------- -->

</main>
</template>

<style scoped>
/* Testing CSS  */
.flex-container {
  display: flex;
  flex-direction: row;
  background: url("src/assets/images/backgroundTransparent.png");
  height: 70vh;
}

.flex-container > div {
  background-color: #f1f1f1;
  width: 100px;
  margin: 10px;
  text-align: center;
  line-height: 75px;
  font-size: 30px;
}

.cardText {
  text-align: left;
  margin-left: 1em;
}

body {
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;

}
.cardName {
  font-weight: 600;
  font-size: 30px;
  margin-left: 1rem;
}

.cardColumn {
  display: flex;
  flex-direction: row;
  align-content: flex-end;
}
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
  /* background-color: rgb(173, 236, 255); */
  text-align: center;

}

/* ----------- Images ------------ */


.cardContainer {
  /* background-color: pink; */
  display: flex;
  align-items: center;
  justify-content: flex-start;
  width: auto;
}


.femaleAvatar {
  width: 8rem;
  margin: 1rem;
  
}

.homeImg {
float: right;
/* display: flex;
flex-direction: column;
margin: auto; */
width: 25rem;
position: relative;
top: -8rem;

}

.arrowImg {
width: 60px;
margin-left: 2rem;
}

.arrowImg:hover {
  border-radius: 15px;
  transition: 0.4;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 5px 8px;
  }



/* ------------------------- */
h2, h1  {
  padding: 1rem;
  color: white;

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

a {
  width: 20%;
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

.madeBtn {
  padding: 0.5em;
  background-color: #37a0c1;
  border: #37a0c1 solid 4px;
  border-radius: 15px;
  text-align: center;
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  font-size: 18px;
  color: white;
}

.madeBtn:hover  {
  border-radius: 15px;
  transition: 0.4;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 5px 8px;
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
  background-image: url("src/assets/images/backgroundTransparentMediaOne.png");
  width: 100%;
  height: 42vh;
}

.homeImg {
/* float: right;
width: 25rem;
position: relative;
top: -8rem;*/
width: 20rem;
} 
h1 {
  font-size: 25px;
}

h2 {
font-size: 15px;
}

.cardName {
  font-size: 25px;
  width: 100%;

}

.cardText {
  font-size: 14px;
  width: 40rem;
  text-align: center;
}

a {
  width: 10%;
}
.madeBtn {
  font-size: 15px;
  display: flex;
  flex-direction: column;
  margin: auto;
}
.femaleAvatar {
  width: 5rem;
}

.meetTitle {
  font-size: 22px;
  width: 100%;
  text-align: center;
}


.slogan {
  font-size: 15px;
}

.learnBtn .galleryBtn {
  font-size: 12px;
}

.arrowImg {
  margin-left: 0;
  margin-right: 400px;
  
  overflow-x: hidden;
  overflow-y: hidden;
}


.cardColumn {
  display: flex;
  flex-direction: column;
  align-content: flex-end;
}
.parent {
  display: flex;
  flex-direction: column;
  
}

.child {
  width: 100%;
  height: 25vh;
  /* background-color: rgb(214, 245, 255); */
  text-align: left;
  color: black;
  padding-left: 1rem;

}
.cardText {
text-align: center;
}

.cardName {
  margin-right: 200px;
  width: 20rem;
}

.femaleAvatar {
  width: 100px;
}

}
</style>
