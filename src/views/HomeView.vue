

<template>
  <main>

<!-- Blue banner home page, displays the slanted blue container with the learnMore button -->
<div class="bgImg container">
  <div class="homeImgContainer">
  <h2>Tech Support Brought to you by</h2>
  <h1 class="brandTitle">Brand name Here</h1>
  
  <img src="src/assets/images/HomeImgTech.svg" alt="img" class="homeImg">

  <hr>
  <h4 class="slogan">Slogan  Lorem ipsum dolor sit amet consectetur adipisicing elit</h4>
<!-- Transition Vue 
ENTERING PAGE
  .enter-from - set intiial css state
  .enter-to - as it enters the browser
  .enter-active - while the element is transitioning from one state to another (time duration)

LEAVING PAGE
.leave-from
.leave-to
.leave-active

TRANSITION NAMES
<transition name="fade">
  .fade-enter-from 
  .fade-enter-to
  .fade-enter-active 
  etc

 -->

 <transition name="fade">
  <div class="transitionTest" v-if="showExample">
    <button class="learnBtn" id="learnMore">Learn more</button>  
    <button class="galleryBtn">Gallery </button>  
  <!-- Toggle inline -->

</div>
</transition>


  <!-- <button @click="showExample = !showExample">toggle</button> -->
</div>

</div>
<button @click="showExample = !showExample">Toggle View</button>




<!-- T -->
<div class="parent">
  <div class="child">
    <h4 class="cardSlogan">Slogan Lorem ipsum dolor sit, amet consectetur adipisicing elit. </h4>
    <h1 class="meetTitle">More than 5,000,000 companies want a website from us</h1>
    <button class="madeBtn">What We've Made</button>
  </div>

  <div class="child2">

    <!-- This is the avatar profile pictuere, that when on hover, it will wave.  -->
    <div class="cardContainer">
      <img :src="femaleAvatarHover" @mouseover="hoverFemaleImg = true" @mouseleave="hoverFemaleImg = false" alt="femaleAvatar" class="femaleAvatar">
      <h3 class="cardName">Bold Name</h3>

  <!-- Button with broken arrow SVG -->
      <a href="about">
      <img src="src/assets/images/arrow.svg" alt="arrow" class="arrowImg">
    </a>
    </div>
    <div class="cardTextContainer">
      <p class="cardText">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat, ipsam alias quas consequuntur aliquam corrupti temporibus incidunt veritatis! Eos tempora nisi officia corrupti dolores ut.</p>
    </div>
  </div>
</div>

<!-- Statistics animation -->
<!-- Bar 1 -->
<div class="statsContainer">
<div class="animationContainer">
  <div class="stats">
    <div class="statsItem">
      <span class="statsPercent">65%</span>
      <div class="statsBar" style="--percentage: 62%;"></div>
      <span class="statsTitle">Something 1</span>
    </div>

<!-- Bar 2 -->
    <div class="statsItem">
      <span class="statsPercent">80%</span>
      <div class="statsBar" style="--percentage: 80%;"></div>
      <span class="statsTitle">Something 2</span>
    </div>
<!-- Bar 3 -->
    <div class="statsItem">
      <span class="statsPercent">90%</span>
      <div class="statsBar" style="--percentage: 90%;"></div>
      <span class="statsTitle">Something 3</span>
    </div>

  </div>
</div>

  <div class="statsTextContainer">
    <div class="statsCard">
      <h2 class="statsCardTitle">Companies "Somethings" improved tremendously. <br> Guaranteed 90% of Something 3!</h2>  
      <div class="modalBtnContainer">
        <button class="modalBtn">See How (Modal Button!)</button>
      </div>
    
    </div>    
  </div>
</div>




</main>
</template>


<script>
export default {
  name: 'HomeView',
  data () {
    return {
      // Variables
      femaleAvatar: "src/assets/images/femaleAvatar.svg",
      femaleAvatarWave: "src/assets/images/femaleAvatarWave.svg",
      hoverFemaleImg: false,
      showExample: false,

    }
  },
  computed: {
    femaleAvatarHover() {
      if(this.hoverFemaleImg == true) {
        return this.femaleAvatarWave
      } else {
        return this.femaleAvatar
      }
    }
  }
}

</script>



<style scoped>
/* ------------ Vue Transition Fade ------------  */
.fade-enter-from {
  opacity: 0;
}

/* Even if we comment this out below, it will still work. This is because the default state IS opacity 1.  */
.fade-enter-to {
  opacity: 1;
  
}

.fade-enter-active {
  transition: all 1s ease;   /*  Can also say "opacity" if you want to transfer JUST the opacity of enter-to */

}


.fade-leave-from {
  opacity: 1;
}

.fade-leave-to {
  opacity: 0;
}

.fade-leave-active {
  transition: all 1s ease;
}



/* ------------ Modal ------------ */
.modalBtnContainer {
  display: flex;
  justify-content: center;
}

.modalBtn {
  padding: 0.5em;
  background-color: #37a0c1;
  border: #37a0c1 solid 4px;
  border-radius: 15px;
  text-align: center;
  font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  font-size: 18px;
  color: white;
  display: flex;
}

.modalBtn:hover {
  border-radius: 15px;
  transition: 0.4s;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 5px 8px;
  justify-content: center;
  align-content: center;
  align-items: center;
  align-self: center;

}

/* ------------ STATS Animation ------------ */
.statsTextContainer {
  /* Child 2 */
  background-color: rgb(221, 237, 255);
  width: 50%;
  display: flex;
  flex-direction: row;
  /* align-items: center; */
  justify-content: flex-end;
  align-content: center;
  align-items: center;
  justify-items: center;

}

.statsCard {
  padding: 50px;
  background: #b3dce9;
  margin: 30px 30px 30px 30px;
  /* align-content: center;
  align-items: center;
  justify-items: center;
  justify-content: center;  
   */

}
.statsCardTitle {
  font-size: 22px;
  text-align: center;
  /* color: #000; */
  font-weight: 600;
}
.statsContainer {
/* This is the parent */
display: flex;
flex-direction: row;
padding: 1rem;
margin-top: 2rem;



}

.stats {
  display: flex;
  justify-content: space-between;
  margin-right: 40%;
  margin-right: 50px;
}


.statsItem {
  text-align: center;
}

.statsBar {
  width: 67px;
  height: 150px;
  margin: 20px 5px;
  border-radius: 4px;
  background: #37A0C1;
  overflow: hidden;
  position: relative;

  width: 80px;
  height: 250px;
  margin: 20px 10px 5px;
  border-radius: 4px;
  background: #37A0C1;
  overflow: hidden;
  position: relative;

}

.statsBar:after {
  content: '';
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: #c7e1e9;
  animation: barsIn 1.5s ease-in-out forwards;
}

.lowerText {
  display: block;
	text-align: left;
	margin-top: 30px;
	opacity: 0.5;
	letter-spacing: 0.5px;
}


@keyframes barsIn {
  0% {
    bottom: 0;
  }
  100% {
    bottom: var(--percentage);
  }
}

/* ------------ Stats animation end ------------  */

/* ------------ Female avatar Card container ------------ */
.cardTextContainer {
  display: flex;
  flex-direction: row;
  align-items: center;
}

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

/* ----------- Images for Female Avatar Card Component ------------ */


.cardContainer {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  width: auto;
}


.femaleAvatar {
  width: 10rem;
  margin: 1rem;
  cursor: pointer;
  
}
/* ----------- Arrow Button for avatar ----------- */
.arrowImg {
width: 60px;
margin-left: 2rem;
}

.arrowImg:hover {
  border-radius: 15px;
  transition: 0.4;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 5px 8px;
  }



/* ----------- Image on top of Blue background Home page ----------- BROKEN */
.homeImg {
float: right;
/* display: flex;
flex-direction: column;
margin: auto; */
width: 25rem;
position: relative;
top: -8rem;

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

h1 {
  font-size: 25px;
}

h2 {
font-size: 15px;
}



a {
  width: 10%;
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
  height: 20vh;
  /* background-color: rgb(214, 245, 255); */
  text-align: left;
  color: black;
  padding-left: 1rem;

}
.cardText  {
text-align: center;
font-size: 14px;
  width: 40rem;
  text-align: center;
}

.cardName {
  width: 20rem;
  text-align: center;
  font-size: 25px;
}



.cardSlogan {
  text-align: center;
  margin-top: 5rem;

}

.femaleAvatar {
  width: 100px;
}

.madeBtn {
  font-size: 15px;
  display: flex;
  flex-direction: column;
  margin: auto;
  margin-top: 20px;

}
.cardContainer {
  justify-content: center;  
  margin-top: 50px;
}

.cardTextContainer {
  display: flex;
  flex-direction: column;
  align-items: center;
}

/* Top section, everything on blue background */

.homeImg {
position: absolute;
margin-top: 210px;
width: 20rem;
margin-bottom: 20px;
top: 0%;

} 

.homeImgContainer {
  display: flex;
  flex-direction: column;
  align-items: center;
}


}
</style>
