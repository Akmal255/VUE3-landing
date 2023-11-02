<template>
  <div class="container">
    <img class="lastimg" src="./assets/images/lastimg.png" alt="">
    <img class="lastimg2" src="./assets/images/lastimg.png" alt="">
    <HeaderComponentVue></HeaderComponentVue>
    <MainComponentVue></MainComponentVue> 
    <FirstSectionComponentVue></FirstSectionComponentVue>
    <SecondSectionComponentVue></SecondSectionComponentVue>
    <ThirdSectionComponentVue></ThirdSectionComponentVue>
    <SwipeComponentVue></SwipeComponentVue> 
    <ClientsComponentVue></ClientsComponentVue>
    <FooterComponentVue></FooterComponentVue>
  </div>
  
</template>

<script>

import HeaderComponentVue from "./components/HeaderComponent.vue";
import MainComponentVue from './components/MainComponent.vue'
import FirstSectionComponentVue from "./components/FirstSectionComponent.vue";
import SecondSectionComponentVue from './components/SecondSectionComponent.vue'
import ThirdSectionComponentVue from './components/ThirdSectionComponent.vue'
import SwipeComponentVue from './components/SwipeComponent.vue'
import ClientsComponentVue from './components/ClientsComponent.vue'
import FooterComponentVue from "./components/FooterComponent.vue";


export default {
  name: 'App',
  components: {
    HeaderComponentVue,
    MainComponentVue,
    FirstSectionComponentVue,
    SecondSectionComponentVue,
    ThirdSectionComponentVue,
    SwipeComponentVue,
    ClientsComponentVue,
    FooterComponentVue,
}
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  border: 0;
  list-style-type: none;
  text-decoration: none;
}
.container{
position: relative;
}
.lastimg{
  position: absolute;
  top: 0;
  right: 0;
  width: 71px;
}
.lastimg2{
  position: absolute;
  top: 1700px;
  left: 0;
  width: 71px;
}
button{
  cursor: pointer;
}

input:focus{
  outline: none;
}
a{
  color: black;
}
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  font: "Poppins";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50; 
  box-sizing: border-box;
}
.container{
  padding: 30px 80px;
}
#app h1{
  font-size: 40px;
  line-height: 36px;
  letter-spacing: 0em;
}
#app h3{
  font-size: 18px;
  line-height: 36px;
  letter-spacing: 0em;
}
#app p{
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0em;

}
@media only screen and (max-width: 430px) {
  .container{
  padding: 16px;
}
.lastimg, .lastimg2{
  display: none;
}
#app h1{
font-size: 24px;
}
}
</style>
