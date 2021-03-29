<template>
  <div id="app">
    <b-navbar>
      <b-navbar-nav class="ml-auto">
        <img id="github" class="navbar-icon" src="./assets/github.svg" alt="GitHub" title="GitHub" onclick="window.open('http://www.github.com/thangplum', '_blank');">
        <img id="linkedin" class="navbar-icon" src="./assets/linkedin.svg" alt="LinkedIn" title="LinkedIn" onclick="window.open('http://www.linkedin.com/in/thangng', '_blank');">
      </b-navbar-nav>
    </b-navbar>
    <b-container fluid>
      <b-row>
        <b-col id="intro-col" cols="12">
          <div class ="intro-wrapper center-it">
            <div id="introTitle" class="main-title">Thang Nguyen</div>
            <div id="introSubtitle" class="sub-title"> Aspiring Computer Science student</div>
            <div id="introLocation" class="sub-title">Galesburg, IL</div>
            <div style="display: inline-block; transform: scale(2.5,1.25);">
              <a id="introArrowButton" class="scroll" @click="scroll">
                <font-awesome-icon id="intro-arrow" :icon="['fas', 'angle-double-down']" />
              </a>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row>
        <b-col id="about-me-col" cols="12">
          <div class="about-me-wrapper">
            <b-card class="mb-2 mx-auto card">
              <b-row>
                <b-col md="4">
                  <b-img id="potrait" fluid thumbnail rounded="circle" :src="require('./assets/cropped-potrait.jpg')" alt="Potrait"></b-img>
                </b-col>
                <b-col md="8">
                  <div class="about-me-title">
                    About Me
                  </div>
                  <div class="about-me-content">
                    My name is Thang Nguyen, and I am a Computer Science student at Knox College. My passion is Computer Science goes back 
                    when my parent got our first computer. Although I started programming only when I came to college, I had tried to exposed 
                    myself to as many fields as possible, from Web Development, Data Science, and Artificial Inteligence. Currently, I am teaching
                    myself the MERN (MongoDB, Express, React.js, Node.js) stack since I enjoy building webapps that have interactive user experience.
                  </div>
                  <div class="about-me-title">
                    Languages, Frameworks, and Libraries 
                  </div>
                  <div class="about-me-tech">
                    <!-- <font-awesome-icon style="" id="react" :icon="['fab', 'react']" /> -->
                    <img src="./assets/react.svg" class="tech"/>
                    <img src="./assets/aws.svg" class="tech"/>
                    <img src="./assets/css.svg" class="tech"/>
                    <img src="./assets/github.svg" class="tech"/>
                    <img src="./assets/html.svg" class="tech"/>
                    <img src="./assets/js.svg" class="tech"/>
                    <img src="./assets/java.svg" class="tech"/>
                    <img src="./assets/python.svg" class="tech"/>
                    <img src="./assets/npm.svg" class="tech"/>
                  </div>
                </b-col>
              </b-row>
            </b-card>
          </div>
        </b-col>
      </b-row>
      <b-row>
        <div id="projTitle" class="sub-title center-it">My work experience</div>
      </b-row>
      <b-row>
        <div class="exp-container">
          <div class="exp-title">Front-end Web Developer Intern</div>
          <div class="exp-text">SaveMoney Corporation (06/2020 - 08/2020)</div>
          <div>
            - Worked with a team of four interns to develop an internal user account management application by using TypeScript, 
React.JS, Node.js and Ant Design Pro
          </div>
          <div>
            - Successfully achieved the purpose for keeping track of current employee accounts, adding or removing policy of current 
employee accounts, and adding new accounts automatically
          </div>
        </div>
        <div class="exp-container">
          <div class="exp-title">Undergraduate Research Assistant</div>
          <div class="exp-text">Vietnam National University Ho Chi Minh City - University of Science (06/2019 - 08/2019)</div>
          <div>
            - Researched virtual reality and its application in helping people with fear of heights
          </div>
          <div>
            - Independently developed Fear the Height, a virtual reality game, that helped people with acrophobia to overcome their fear 
            using Microsoft Mixed Reality Toolkit, Google VR Daydream library, and Unity; the core gameplay was fully 
            implemented and tested
          </div>
        </div>
        
        <div class="exp-container">
          <div class="exp-title">Front-end Web Developer</div>
          <div class="exp-text">Startup Term, Knox College (03/2019 - 05/2019)</div>
          <div>
            - Professionally collaborated with 4 other developers to build a social networking website with JavaScript, 
            React.JS, Bootstrap and Node.js and hosted on Amazon Web Services, including forums, messenger and livestream 
            video and more
          </div>
          <div>
            - Received the prestigious award Stroben Prize for Entrepreneurship from Knox College as an incubator award
          </div>
        </div>
        <div class="exp-container">
          <div class="exp-title">Computer Science Tutor</div>
          <div class="exp-text">SaveMoney Corporation (09/2019 - Present)</div>
          <div>
            - Evaluated by the tutees and the tutoring center as one of the most effective tutors with an average effectiveness 
            9.71/10 with 21 students
          </div>
          <div>
            - Supported and assisted students from all Computer Science classes with their in-class coursework, homework, and how 
            they could improve on understanding concepts and how to use them
          </div>
          <div>
            - Exceed all personal and team goals while maintaining positive feedback from all students and fellow tutors
          </div>
        </div>
      </b-row>
      <b-row>
        <div id="projTitle" class="sub-title center-it">My projects</div>
      </b-row>
      <b-card-group deck>
        <b-card title="Spoticlone" :img-src="require('./assets/spoticlone.png')" img-alt="Image" img-top onclick="window.open('https://spoticlone-thangng.netlify.app', '_blank');">
          <b-card-text>
            A functional clone of Spotify front-end consumes data from the Spotify API and tries to mimic the UI 
            and front-end behaviors of the official Spotify web player using React.JS, axios, Node.js, Express, TypeScript.
          </b-card-text>
        </b-card>
        <b-card title="Covid Tracker" :img-src="require('./assets/covid-tracker.png')" img-alt="Image" img-top onclick="window.open('https://github.com/thangplum/covid-tracker', '_blank');">
          <b-card-text>
            A web-app that lets users keep track of the current number of patients and deceased of COVID-19 at the moment either globally 
            or nationally with an attractive interface using React/Redux, JavaScript, and Node.js
          </b-card-text>
        </b-card>
        <b-card title="My Portfolio" :img-src="require('./assets/portfolio.png')" img-alt="Image" img-top>
          <b-card-text>
            I made this web-portfolio to increase my web presence, and test my abilities in web design.
            This web-app used Vue, Vue-Bootstrap, and JavaScript.
          </b-card-text> 
        </b-card>
      </b-card-group>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    
  },
  methods: {
    scroll() {
      const element = document.getElementById('about-me-col');
      element.scrollIntoView({ behavior: 'smooth' });
    }
  }
}
</script>

<style>
#app {
  background: linear-gradient(#084e74,#53addd);
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  min-height: 100vh;
  padding-right: 3vw;
  padding-left: 3vw;
  padding-bottom: 0px;
}

.navbar-icon{
  margin-top: 2px;
  margin-left: 6px;
  margin-right: 6px;
  height: 2.5em;
  width: 2.5em;
}

.navbar-icon:hover{
  transform: translateY(55px);
  -webkit-transform: translateY(5px);
  transition-duration: 0.2s;
  cursor: pointer;
  width: 2.75em;
  height: 2.75em;
}

#intro-col{
  padding: 0px !important;
  margin: 0px !important;
}

.intro-wrapper{
  /* background: linear-gradient(#041c29,#08486B); */
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: auto 100%;
  background-repeat: no-repeat;
  width: 100%;
  min-height: 80vh;
  padding-right: 35px;
  padding-left: 35px;
  padding-bottom: 0px;
}

.center-it {
  margin:0 auto;
  text-align: center;
}

.main-title {
  margin-top: 25vh;
  margin-bottom: 5vh;
  font-family: 'Pridi', serif;
  font-size: min(20vw, 75px);
  color: #ffef9b;
  line-height: 75%;
}

.sub-title {
  line-height: 100%;
  margin-bottom: 5px;
  font-size: min(4.5vw, 35px);
  color: #ffef9b;
  font-family: 'Montserrat', sans-serif;  
}

#intro-arrow{
  font-size:2em; 
  color:#ffef9b;
  margin-top: 7vh; 
  display: inline-block;
  transform: scale(2.25,1.5);
}

.about-me-wrapper {
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  align-content: center;
}

.about-me-title {
  margin-top: 2px;
  margin-bottom: 5px;
  font-family: 'Pridi', serif;
  font-size: min(5vw, 25px);
  border-bottom: 2px solid #12849f;
  font-weight: 700;
}

.about-me-content {
  font-family: 'Pridi', serif;
  margin-bottom: 2vw;
  font-size: min(4vw, 20px);
}

.about-me-tech {
  text-align: center;
}

.tech {
  width: 3em;
  height: 3em;
  margin: 2px;
}

.card {
  width: 100%;
  height: 100%;
  max-width: 1000px;
}

#projTitle {
  text-align: center;
  font-size: min(60px, 10vw);
  margin-top: 20px;
  margin-bottom: 20px;
}

.exp-container {
  width: 100%;
  margin-bottom: 10px;
  margin-left: 6vw;
  margin-right: 6vw;
}

.exp-title {
  font-size: min(5vw, 25px);
  font-weight: 700;
}

.exp-text {
  font-size: min(4vw, 20px);
  font-style: italic;
}

.exp-subtitle {
  font-size: min(3vw, 15px);
}
</style>
