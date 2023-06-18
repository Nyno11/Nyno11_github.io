<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css">

<style>
@import url('https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css');
@import url('https://fonts.googleapis.com/css2?family=Fraunces:opsz@9..144&family=Roboto:wght@400&display=swap');

/* Basic Css */

* {
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  outline: none;
  border: none;
  text-decoration: none;
  /* text-transform: capitalize; */
  transition: all 0.2s linear;
  /* color: #a1b2b1; */
  color: black;
  line-height: 1.6em;
}

/* The Main container  */

.main-container {
  height: 100vh;
  width: 100%;
}

html {
  font-size: 62.5%;
  overflow-x: hidden;
}

body {
  background-color: #eae4d7;
  margin: 0px;
}

/* Styling the header : Navigation Bar */

header {
  margin: 0px;
}

a {
  text-decoration: none;
  color: #195cc8;
  font-weight: bold;
}

ul {
  list-style: none;
}

section {
  padding: 2rem 9%;
}

.logo {
  font-size: 2.5rem;
  font-weight: bolder;
  display: inline-block;
}

.logo i {
  padding-right: 2rem;
  color: black;
}

.logo {
  font-size: 35px;
  letter-spacing: 1px;
  cursor: pointer;
}

span {
  color: #195cc8;
}

.span2 {
  font-family: 'Fraunces', serif;
}

/* Styling the nav container */

.nav {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  background-color: #eae4d7;
  height: 65px;
  font-size: 20px;
  padding-left: 8%;
  padding-right: 8%;
}

.menu li:hover {
  cursor: pointer;
  transform: scale(1.2);
}

.menu {
  display: flex;
  flex-direction: row;
  list-style-type: none;
  margin: 0;
}

.menu > li {
  margin: 0 1rem;
  overflow: hidden;
}

/*Container for menu button  */

.menu-button-container {
  display: none;
  height: 100%;
  width: 30px;
  cursor: pointer;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

#menu-toggle {
  display: none;
}

/*  Creating the menu button */

.menu-button,
.menu-button::before,
.menu-button::after {
  display: block;
  /* background-color: white; */
  background-color: #195cc8;
  position: absolute;
  height: 6px;
  width: 32px;
  border-radius: 3px;
  color: black;
}

.menu-button::before {
  content: '';
  margin-top: -8px;
}

.menu-button::after {
  content: '';
  margin-top: 8px;
}

/*  Adding Functionality to the Hamburger Menu with CSS  */

#menu-toggle:checked + .menu-button-container .menu-button::before {
  margin-top: 0px;
  transform: rotate(45deg);
}

#menu-toggle:checked + .menu-button-container .menu-button {
  background: rgba(255, 255, 255, 0);
}

#menu-toggle:checked + .menu-button-container .menu-button::after {
  margin-top: 0px;
  /*  transforms the hamburger icon into a cross  */
  transform: rotate(-45deg);
}

/* Styling the hero section */

.hero {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  height: calc(100% - 65px);
  align-items: center;
  background-color: #eae4d7;
}

/* Styling the hero image */

.hero .image {
  flex: 1 1 30rem;
}

.hero .image img {
  width: 100%;
  height: 100%;
  padding: 1rem;
  animation: float 3s linear infinite;
}

/* animating the main image   */

@keyframes float {
  0%,
  100% {
    transform: translateY(0rem);
  }
  50% {
    transform: translateY(3rem);
  }
}

/* Styling the buttons for the hero and about section */

button {
  background-color: transparent;
  color: #195cc8;
  text-decoration: none;
  border: 2px solid black;
  font-weight: bold;
  font-size: 15px;
  padding: 13px 30px;
  border-radius: 30px;
  transition: 0.4s;
}

.btn1,
.btn2 {
  margin: 1rem;
}

.btn1 {
  background-color: #195cc8;
  color: white;
  border: none;
  padding: 15px 32px;
}

button:hover {
  opacity: 0.6;
  cursor: pointer;
}

/* herocontent hero section */

.herocontent {
  margin: auto;
}

.hero .herocontent {
  flex: 1 1 40rem;
}

h1 {
  color: black;
  margin: 20px 0px 20px;
  font-size: 80px;
  font-family: 'Fraunces', serif;
  letter-spacing: 2px;
}

.surname {
  font-family: 'Fraunces', serif;
}

h2 {
  color: black;
  font-size: 35px;
  margin-bottom: 15px;
}

h4 {
  letter-spacing: 2px;
  font-size: 20px;
}

h3 {
  font-size: 30px;
  color: black;
  letter-spacing: 2px;
}

.tag2 {
  margin-top: 5px;
  margin-bottom: 30px;
}

.hero p {
  font-size: 25px;
}

/*Styling the About section*/

.about {
  width: 100%;
  height: 100vh;
  padding: 150px 0px;
  background-color: #e8e9e3;
}

.about img {
  height: auto;
  width: 430px;
  border-radius: 30px;
  box-shadow: rgba(26, 24, 24, 0.25) 0px 5px 10px 2px;
}

.about-text {
  width: 550px;
}

/* about container */

.main {
  width: 1130px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.about-text h2 {
  font-size: 50px;
  text-transform: capitalize;
  margin-bottom: 20px;
  font-weight: bold;
  color: #195cc8;
  font-family: 'Fraunces', serif;
}

.about-text h5 {
  letter-spacing: 2px;
  font-size: 22px;
  margin-bottom: 25px;
  text-transform: capitalize;
  font-weight: bold;
  color: black;
  font-family: 'Frances', serif;
}

.about-text p {
  letter-spacing: 1px;
  line-height: 28px;
  font-size: 18px;
  margin-bottom: 45px;
}

/*
Skills 

*/

/* skills section styling */

.skills {
  height: 100vh;
}

.skills .skills-content {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

section .title {
  position: relative;
  text-align: center;
  font-size: 50px;
  font-weight: bold;
  margin-bottom: 85px;
  padding-bottom: 20px;
  letter-spacing: 1px;
  font-family: 'Fraunces', serif;
  color: #195cc8;
}

.skills .title::after {
  content: '';
  position: absolute;
  bottom: 0px;
  left: 50%;
  width: 180px;
  height: 3px;
  background: black;
  transform: translateX(-50%);
}

.skills .skills-content .column {
  width: calc(50% - 30px);
}

.skills .skills-content .left .text {
  font-size: 40px;
  font-weight: 600;
  margin-bottom: 10px;
}

.skills .skills-content .left p {
  text-align: justify;
  font-size: 18px;
}

.skills .skills-content .left a {
  display: inline-block;
  background: rgb(57, 95, 165);
  color: #fff;
  font-size: 18px;
  font-weight: 500;
  padding: 8px 16px;
  margin-top: 20px;
  border-radius: 6px;
  border: 2px solid rgb(57, 95, 165);
  transition: all 0.3s ease;
}

.skills .skills-content .left a:hover {
  color: rgb(57, 95, 165);
  background: none;
}

.skills .skills-content .right .bars {
  margin-bottom: 15px;
}

.skills .skills-content .right .info {
  display: flex;
  margin-bottom: 5px;
  align-items: center;
  justify-content: space-between;
  animation: slide 2s ease-in-out;
}
@keyframes slide {
  0%{
    transform:translateX(-100px);
    opacity: 0;
    
  }
}

.skills .skills-content .right span {
  font-weight: 500;
  font-size: 18px;
}

.skills .skills-content .right .line {
  position: relative;
  border: 1px solid #504f4f;
  padding: 5px;
  border-radius: 10px;
  height: 10px;
  background: #504f4f;
}

.skills .skills-content .right .progressBar {
  border: 1px solid #504f4f;
  padding: 5px;
  border-radius: 10px;
}

.skills .skills-content .right .line::before {
  content: '';
  position: absolute;
  height: 100%;
  left: 0;
  top: 0;
  /* background: rgb(57, 95, 165); */
  transition: width 0.6s ease;
  height: 10px;
  border-radius: 5px;
  vertical-align: middle;
  align-self: center;
  background-image: -moz-linear-gradient(0deg, #3a6dc1 0%, #195cc8 100%);
  background-image: -webkit-linear-gradient(0deg, #3a6dc1 0%, #195cc8 100%);
  color: #195cc8;
  animation: slide 2s ease-in-out;
}
@keyframes slide {
  0%{
    transform:translateX(-100px);
    opacity: 0;
    
  }
}

.skills-content .right .mern::before {
  width: 92%;
  animation: slide 2s ease-in-out;
}
  
@keyframes slide {
  0%{
    transform:translateX(-100px);
    opacity: 0;
    
  }
}

.skills-content .right .js::before {
  width: 88%;
}

.skills-content .right .react::before {
  width: 75%;
}

.skills-content .right .wireframing::before {
  width: 70%;
}

.skills-content .right .prototyping::before {
  width: 85%;
}

.skills-content .right .figma::before {
  width: 75%;
}

.max-width {
  max-width: 1300px;
  padding: 0 80px;
  margin: auto;
}

.headbar {
  background: none;
  color: black;
  animation: slide 3s ease-in;
}
@keyframes slide {
  0%{
    transform:translateX(-100px);
    opacity: 0;
    
  }
}

/* project */

.project {
  background-color: rgb(232, 233, 227);
  width: 100%;
  padding: 100px 0px;
  height: 100px;
}

.box {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 400px;
  border-radius: 20px;
}

.flip-card {
  background-color: transparent;
  width: 335px;
  height: 365px;
  perspective: 1000px;
  padding: 20px 35px;
  text-align: center;
  align-items: center;
  border-radius: 20px;
  margin: 15px;
  position: relative;
  
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 2);
  border-radius: 20px;
}


.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}


.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  border-radius: 10px;
}

.flip-card-front {
  background-color: rgb(23, 7, 246);
  color: rgb(25, 2, 113);
}

.flip-card-back {
  background-color: #ffffff;
  color: white;
  transform: rotateY(180deg);
}



.CV-page {
  max-width: 800px;
  height: 100vh;
  margin: 0 auto;
  padding: 0 2em;
  color: #222222;
  font-size: 1em;
  font-family: 'Lato', sans-serif;
}

.CV-secondaryHeading {
  position: relative;
  margin: 1em 0 0;
  margin-bottom: 40px;
  padding-bottom: 20px;
  text-align: center;
  font-weight: bold;
  font-size: 50px;
  color: #195cc8;
  font-family: 'Fraunces', serif;
}

.CV-secondaryHeading::after {
  content: '';
  position: absolute;
  bottom: 0px;
  left: 50%;
  width: 180px;
  height: 3px;
  background-color: #111;
  transform: translateX(-50%);
  margin-top: 10px;
}

.CV-grid {
  display: table;
}

.CV-grid-column {
  display: table-cell;
}

.CV-timeline {
  position: relative;
  margin: 0 0 0 0.5em;
  padding-left: 1.5em;
  border-left: solid 1px #a1b2b1;
}

.CV-timeline:first-of-type {
  margin-top: 1em;
}

.CV-timeline:last-of-type {
  border-left-color: transparent;
}

.CV-timeline:before {
  content: '';
  position: absolute;
  top: 0;
  left: -0.5em;
  display: block;
  width: 1em;
  height: 1em;
  border: solid 1px #222222;
  background-color: #ffffff;
  border-radius: 50%;
}

.CV-timeline-heading {
  margin: 0;
  padding-bottom: 0.5em;
  line-height: 1em;
  font-weight: normal;
  -webkit-transform: translateY(-0.1em);
  -ms-transform: translateY(-0.1em);
  transform: translateY(-0.1em);
}

.CV-timeline-heading-title {
  line-height: 1;
  font-style: italic;
  text-transform: uppercase;
  /* background: none;
    -webkit-text-fill-color: #249f9f;
    -webkit-background-clip: text; */
}

.CV-timeline-heading-location {
  font-size: 0.8em;
  background: none;
  /* -webkit-text-fill-color: #a1b2b1;
    -webkit-background-clip: text; */
  color: #111;
}

.CV-timeline-heading-duration {
  display: block;
  font-size: 0.7em;
  background: none;
  -webkit-text-fill-color: #6f6f6f;
  -webkit-background-clip: text;
}

.CV-timeline-details {
  display: block;
  margin: 0;
  padding-bottom: 2em;
  padding: 0 0 1em 1em;
  list-style-type: disc;
  font-size: 15px;
}

.CV-timeline-details-item,
.CV-job-timeline-item {
  margin-bottom: 0.3em;
}

/* service */

.service {
  background-color: rgb(232, 233, 227);
  width: 100%;
  padding: 100px 0px;
  height: 100vh;
}

.title h2 {
  font-size: 50px;
  margin: 30px auto;
  text-align: center;
  font-weight: 500;
  color: #195cc8;
  font-family: 'Fraunces', serif;
}

.title h2 ::after {
  content: '';
  position: absolute;
  bottom: 0px;
  left: 50%;
  width: 180px;
  height: 3px;
  background: rgb(161, 178, 177);
  transform: translateX(-50%);
  margin-top: 10px;
}

.box {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 400px;
  
}

.card {
  height: 365px;
  width: 335px;
  padding: 20px 35px;
  background-color: rgb(232, 233, 227);
  border-radius: 20px;
  margin: 15px;
  position: relative;
  overflow: hidden;
  text-align: center;
  box-shadow: rgb(26 24 24 / 25%) 0px 5px 10px 2px;
  
}

.card i {
  font-size: 50px;
  display: block;
  text-align: center;
  margin: 25px 0px;
  color: #f9004d;
  
}

h5 {
  color: #195cc8;
  font-size: 23px;
  margin-bottom: 15px;
}

.pra p {
  font-size: 18px;
  line-height: 27px;
  margin-bottom: 25px;
}

.card .button {
  background-color: transparent;
  color: #195cc8;
  text-decoration: none;
  border: 2px solid black;
  font-weight: bold;
  padding: 9px 22px;
  border-radius: 30px;
  animation: slide 3s ease-in;
}

@keyframes slide {
  0%{
    transform:translateX(-100px);
    opacity: 0;
    
  }
}

.card .button:hover {
  background-color: transparent;
  border: 2px solid #249f9f;
  cursor: pointer;
}

/* contact me  */

.contact {
  height: 100vh;
}

.contactUs {
  position: relative;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 4%;
  margin-bottom: 5%;
}

.contact-box {
  max-width: 850px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #fff;
  box-shadow: 0px 0px 19px 5px rgb(124, 122, 122);
}

.contactLeft {
  background-color: rgba(230, 230, 230, 0.6);
  height: 100%;
}

.contactRight {
  padding: 25px 40px;
  /* background: #191919; */
}

.contact-content {
  font-size: 17px;
  margin: 1rem;
}

.contacth2 {
  position: relative;
  padding: 0 0 10px;
  margin-bottom: 10px;
  font-weight: 500;
  color: black;
}

.contact-img {
  margin: 1rem;
  border-radius: 100%;
  width: 200px;
  height: 200px;
}

.contactField {
  width: 100%;
  border: 2px solid rgba(0, 0, 0, 0);
  outline: none;
  background-color: rgba(230, 230, 230, 0.6);
  padding: 1rem 1rem;
  font-size: 1.5rem;
  margin-bottom: 22px;
  transition: 0.3s;
}

.contactField:hover {
  background-color: rgba(0, 0, 0, 0.1);
}

.contactTextarea {
  min-height: 150px;
}

.contactBtn {
  width: 100%;
  padding: 0.5rem 1rem;
  background-color: transparent;
  border: 2px solid black;
  font-size: 1.5rem;
  outline: none;
  cursor: pointer;
  transition: 0.3s;
  color: black;
}

.contact-info {
  font-size: 20px;
  text-align: center;
  padding: 1rem;
  text-align: justify;
  margin-left: 20%;
}

.contact-info p {
  color: black;
  margin: 1rem;
}

.contactField:focus {
  border: 2px solid rgb(33, 31, 47);
  background-color: white;
}

.contactTitle {
  text-align: center;
  font-size: 50px;
  font-weight: 500;
  color: #195cc8;
  font-family: 'Fraunces', serif;
}

/* footer */

.social_icon {
  text-align:center;

}

.social_icon ul{
  list-style: none;
  padding-left: 400px;

}

     /*twitter*/
.social_icon ul li:hover.twitter {
transform: scale(1.2);
}

.social_icon ul li:hover.bi-twitter {
  transform: scale(1.2);
}

       /*whatsapp*/
.social_icon ul li:hover.whatsapp {
transform: scale(1.2);
}

.social_icon ul li:hover.bi-whatsapp {
  transform: scale(1.2);
}

     /*envelope*/
.social_icon ul li:hover.envelope{
transform: scale(1.2);
}

.social_icon ul li:hover.bi-envelope {
  transform: scale(1.2);
}
   
      /*github*/
.social_icon ul li:hover.github{
transform: scale(1.2);
}

.social_icon ul li:hover.bi-github {
  transform: scale(1.2);
}

  /*linkedin*/
.social_icon ul li:hover.linkedin{
transform: scale(1.2);
}

.social_icon ul li:hover.bi-linkedin {
  transform: scale(1.2);
}

.footertext {
  font-size: 25px;
  color: rgb(69, 12, 213);
  font-weight: bold;
  text-align: center;
}

/* media queries  */

@media (max-width: 991px) {
  html {
    font-size: 55%;
  }
  header {
    padding: 2rem;
  }
  section {
    padding: 2rem;
  }
}

@media screen and (max-width: 880px) {
  .contact-box {
    grid-template-columns: 1fr;
  }
  .contactLeft {
    height: 100%;
  }
  .about img {
    display: none;
  }
  html {
    font-size: 50%;
    overflow-x: hidden;
    overflow-y: scroll;
  }
  .main {
    width: 100%;
  }
  .box {
    display: block;
  }
  .card {
    margin: 15px auto;
  }
  .service {
    height: fit-content;
  }
  .contact {
    height: fit-content;
  }
}

@media (max-width: 768px) {
  .menu-button-container {
    display: flex;
  }
  a {
    color: black;
  }
  .menu {
    position: absolute;
    top: 0;
    margin-top: 50px;
    left: 0;
    flex-direction: column;
    width: 100%;
    justify-content: center;
    align-items: center;
    padding: 2rem;
    z-index: 2;
  }
  .menu li:hover {
    transform: scale(1.2);
  }
  #menu-toggle ~ .menu li {
    height: 0;
    margin: 0;
    padding: 0;
    border: 0;
  }
  #menu-toggle:checked ~ .menu li {
    border: 1px solid #9f9a9a;
    height: 2.5em;
    padding: 0.5em;
  }
  .menu > li {
    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0.5em 0;
    width: 100%;
    color: black;
    background-color: #e8e8e8;
  }
  .menu > li:not(:last-child) {
    border-bottom: 1px solid #444;
  }
  .logo i {
    color: white;
  }
  .about img {
    display: none;
  }
  .main {
    width: 100%;
  }
}

@media (max-width: 450px) {
  html {
    font-size: 50%;
    overflow-x: hidden;
    overflow-y: scroll;
    text-align: center;
  }
  h1 {
    font-size: 60px;
  }
  h2 {
    font-size: 40px;
  }
  h3 {
    font-size: 17px;
  }
  .service {
    height: fit-content;
  }
  .box {
    display: block;
  }
  .card {
    margin: 15px auto;
  }
  .CV-page {
    height: fit-content;
  }
  .contact {
    height: fit-content;
    margin: 1rem;
    padding: 0;
  }
  section .title {
    font-size: 60px;
  }
  .max-width {
    padding: 0;
    max-width: fit-content;
  }
  .CV-page {
    padding: 0 1em;
  }
}

</style>
</head>

<body>
    <div class="main-container">
        <!-- header section starts  -->

        <header>
            <section class="nav">
                <!-- We can also insert any logo here     -->

                <!-- We can also insert any logo here     -->
                <div class="logo">
                    <h2 class="logo">NY<span>NO</span></h2>
                </div>

                <!--  checkbox to control the icon's state    -->
                <input id="menu-toggle" type="checkbox" />
                <label class="menu-button-container" for="menu-toggle">
        <div class="menu-button"></div>
      </label>
                <!--  main menu    -->
                <ul class="menu">
                    <li><a href="#hero">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact">Contact me</a></li>
                </ul>
            </section>
        </header>

        <!-- header section ends -->
        <section class="hero" id="hero">


            <!----hero Section start---->

            <div class="herocontent">
                <h4>Hello , Nice to see you! I'm</h4>
                <h1>F<span class="surname">R</span>A<span>N</span>K<span>L</span>I<span>N</span> O<span>B</span>I<span>O</span>R<span>A</span></h1>
                <h2>I'm a web designer and front-end developer.</h2>
                <h3>Creating Elegant <span class="span2">DESIGNS</span> beyond just </h3>
                <h3 class="tag2">putting <span class="span2">PIXELS</span> together.</h3>

                <a href="franklinobiora20@gmail.com:#"><i class=""></i> <button class="btn1">Hire Me</button></a>
                <a href="C:\Users\frank\RD\myporfolio\Copy-Franklin's Resume.pdf"><button class="btn2">Resume<i class="bi bi-download"></i></button></a>


            </div>

            <div class="image">
                <img src="programming (1).png" alt=" " />
            </div>

        </section>
        <!-- hero section ends -->


        <!----About section start---->
        <section class="about" id="about">
            <div class="main">
                <img src="C:\Users\frank\RD\myporfolio\profile-pic (1).png" class="aboutimg">
                <div class="about-text">
                    <h2>About Me</h2>
                    <h5>Web designer and front-end developer</h5>
                    <p>My name's Franklin, #codename Nyno. I'm a Web designer and front-end developer based in Nigeria, Africa.
<br>
<br>
                      I work as a Lead developer, freelancer, SDG Advocate (Community Service) and also utilize part of my time to build personal projects. I spend my leisure hours in reading, exercising, playing sports and video games. Currently, practising my skills at machine learning and AI. I love to learn and explore new areas, languages and frameworks. 
                    </p>
                    <a href="#contact"><button type="submit">Let's Talk</button></a>
                </div>
            </div>
        </section>
        <!-- About section ends -->

        <!-- skills section start -->
        <section class="skills" id="skills">
            <div class="max-width">
                <h2 class="title">Key Skills</h2>
                <div class="skills-content">
                    <div class="column right">
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">HTML5,CSS3,Bootstrap</span>

                            </div>
                            <div class="progressBar">
                                <div class="line mern"></div>
                            </div>
                        </div>
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">Javascript(ES6)</span>

                            </div>
                            <div class="progressBar">
                                <div class="line js"></div>
                            </div>

                        </div>
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">React.js</span>

                            </div>
                            <div class="progressBar">
                                <div class="line react"></div>
                            </div>
                        </div>
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">Wireframing</span>

                            </div>
                            <div class="progressBar">
                                <div class="line mongo"></div>
                            </div>
                        </div>
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">Prototyping</span>

                            </div>
                            <div class="progressBar">
                                <div class="line node"></div>
                            </div>

                        </div>
                        <div class="bars">
                            <div class="info">
                                <span class="headbar">Figma ,Adobe XD ,Maze </span>

                            </div>
                            <div class="progressBar">
                                <div class="line corecs"></div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!--skills section ends   -->

        <!-- Projects section -->

        <div class="service" id="projects">
            <div class="title">
                <h2 class="project-heading">Projects</h2>
            </div>

            <div class="box">
             
               
                <div class="flip-card">
               
                  <div class="flip-card-inner">
             
                    <div class="flip-card-front">
                <img src="C:\Users\frank\RD\myporfolio\image2 (1) (1).jpeg" alt="Encyclo podcast" style="width: 250px;height: 250px;">
              <h1 style="font-size: 15px;">VERBAL VOYAGE</h1>      
              </div>
                <div class="flip-card-back">
                  <h1 style="font-size: 15px;">VERBAL VOYAGE</h1>
                  <div class="pra">
                  <P>Verbal Voyage is a podcast that takes a deep dive into the most important societal issues of our time. From current events and personal development to technology, pop culture, and entrepreneurship, we cover it all.</P>
                </div>
                </div>
              
              </div>
          </div>
        
      
    
               
                   <div class="flip-card">
         
                    <div class="flip-card-inner">
       
                      <div class="flip-card-front">
                       <img src="C:\Users\frank\RD\myporfolio\image1 (1) (1).jpeg" alt="BeHealthy" style="width: 250px;height: 250px;">
                      <h1 style="font-size: 15px;">BEHEALTHY</h1>
                      </div>
                            <div class="flip-card-back">
                          <h1 style="font-size: 15px;">BEHEALTHY</h1>
                          <div class="pra">
                         <P>Behealthy is an organization that helps her clients to live healthier and sustainable lives and also make the health system work better for everybody.</P>
                             </div>
                            </div>
                 </div>
             </div>
          
      


               
    <div class="flip-card">
   
      <div class="flip-card-inner">
 
        <div class="flip-card-front">
    <img src="C:\Users\frank\RD\myporfolio\image0 (3) (1).jpeg" alt="logo" style="width: 250px;height: 250px;">
    <h1 style="font-size: 15px;">NIDAS</h1>  
  </div>
    <div class="flip-card-back">
      <h1 style="font-size: 15px;">NIDAS</h1>
      <div class="pra">
      <P>Nidas provides customers with suitable inner wears and fashionable outfit. We provide for both male and female, also for little children and babies.</P>
    </div>
    </div> 
  
  </div>
</div>

      
      </div>
    </div>
             
        <!-- Project section ends  -->

        <!-- Services section starts -->
        <div class="service" id="services" style="background-color: #eae4d7;">
          <div class="title">
              <h2 class="service-heading">Services</h2>
              <p style="text-align: center; font-size: 20px; color: #111215;">I Provide The Best In Class Services For My Clients, And These Are Some Of The Services I Offer.</p>
         
            </div>
<br>
          <div class="box">
              <div class="card">
                  <i class="fas fa-bars"></i>
                  <h5>Web development</h5>
                  <div class="pra">
                    <img src="C:\Users\frank\RD\myportfolio\icons8-web-development-64.png"  style="height: 200px; width: 200px; animation: float 3s linear infinite; ">

                  </div>
              </div>

              <div class="card">
                  <i class="far fa-user"></i>
                  <h5>Web design</h5>
                  <div class="pra">
                     <img src="C:\Users\frank\RD\myportfolio\icons8-web-design-64.png" style="height: 160px; width: 160px;animation: float 3s linear infinite;">

                  </div>
              </div>

              <div class="card">
                  <i class="far fa-bell"></i>
                  <h5>Blockchain development</h5>
                  <div class="pra">
                      <img src="C:\Users\frank\RD\myportfolio\icons8-blockchain-technology-64.png" style="height: 180px; width: 180px; animation:float 3s linear infinite;">
                 
                    </div>
              </div>
          </div>
      </div>

        
        <!-- Services section ends  -->

        <!-- Testimonials section starts  -->
        <div class="service" id="testimonials">
            <div class="title">
                <h2 class="testimonial-heading">Testimonials</h2>
            </div>

            <div class="box">
                <div class="card">
                    <i class="fas fa-bars"></i>
                    <img src="C:\Users\frank\RD\myporfolio\image2 (2).jpeg" alt="Avatar" class="avatar" style="height: 100px; width: 100px; ">
                    <h5 style="font-size: 20px;">Maxwell (project Manager)</progress></h5>
                    <div class="pra">
                        <p>Franklin is an impressive and professional web developer that I have had the pleasure to work with.</p>
                       
                    </div>
                </div>

                <div class="card">
                    <i class="far fa-user"></i>
                    <img src="C:\Users\frank\RD\myporfolio\man (1).png" alt="Avatar" class="avatar" style="height: 100px; width: 100px;">
                    <h5 style="font-size: 20px;">Taofeeq (Mobile developer)</h5>
                    <div class="pra">
                        <p>It's always a pleasure working with Franklin, he's good at communicating and delivering good results. He brings 100% to each project and gets workdone when it's needed the most.</p>
                      
                    </div>
                </div>

                <div class="card">
                    <i class="far fa-bell"></i>
                    <img src="C:\Users\frank\RD\myporfolio\woman (1).png" alt="Avatar" class="avatar" style="height: 100px; width: 100px;">
                    <h5 style="font-size: 20px;">Jennifer (IT officer)</h5>
                    <div class="pra">
                        <p>He shows good understanding of clients needs and deliver top products.</p>
                       
                    </div>
                </div>
            </div>
        </div>

        <!-- Testimonials section ends -->

        <!-- contact us section starts  -->
        <section class="contact" id="contact">

            <h2 class="contactTitle">Contact Me</h2>
            <div class="container contactUs">

                <div class="contact-box">
                    <div class="left contactLeft">
                        <img src="C:\Users\frank\RD\myporfolio\profile-pic (1).png" class="contact-img" alt="" width="150px " />

                        <div class="contact-info">
                            <p><i class="bi bi-telephone-fill"></i> +2349039272958</p>
                            <p><i class="bi bi-envelope-fill"> </i>franklinobiora20@gmail.com</p>
                            <p><i class="bi bi-geo-alt-fill"></i>Port-Harcourt, Nigeria</p>

                        </div>
                        <p class='contact-content'>If you have any queries at all, please feel free to reach out and I'll gladly answer them. </p>

                        <p class='contact-content'>Thanks for visiting .</p>

                    </div>
                    <div class="right contactRight">
                        <h2 class='contacth2'>Lets Connect</h2>
                        <form>
                            <input type="text" class="field contactField" placeholder="Enter your Full Name" required/>
                            <input type="email" class="field contactField" placeholder="Enter your Email" required/>
                            <input type="text" class="field contactField" placeholder="Enter your Phone Number" />
                            <textarea name="msg" placeholder="Suggestions/Queries" class="field contactField contactTextarea" required></textarea>
                            <button class="btn contactBtn" type='submit'>Send</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
        <!-- contact section ends -->

        <!-- Footer -->

        <section id="social_icon">

                <div class="social_icon">
                   
                  <ul class="menu">
                   <li class="twitter"> <a href="https://twitter.com/11_frankie"><i class="bi bi-twitter social" style="font-size: 80px; text-align: center; color: blue;"></i></a></li>
                    <li class="whatsapp"><a href="https://wa.me/2349039272958"><i class="bi bi-whatsapp social" style="font-size: 80px; text-align: center; color: green;"></i></a></li>
                    <li class="envelope"><a href="franklinobiora20@gmail.com"><i class=" bi bi-envelope social" style="font-size: 80px; color: #4a6591;"></i></a></li>
                    <li class="github"><a href="https://github.com/Nyno11"><i class=" bi bi-github" style="font-size: 80px; color: #0d0d0e;"></i></a></li>
                    <li class="linkedin"><a href="https://www.linkedin.com/in/franklin-obiora-9117177"><i class=" bi bi-linkedin social" style="font-size: 80px; color: #4a6591;"></i></a></li>
                  </ul>
                  </div>
        </section>
        <p class="footertext">© Designed by @Nyno</p> 
    </div>

    
</body>

</html>
