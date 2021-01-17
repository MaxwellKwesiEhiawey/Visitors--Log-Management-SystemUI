<template>
  <div class="hello">
    <h1 class="welcome-msg">{{ msg }}</h1>
    <!-- <p>
     Please Select the an Option<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p> -->
    
 <h3 class="header">Please Select and Input as Applied </h3>
    <div class="button">
      <router-link >
 <button class="btn">Staff Sign In</button>
      </router-link>
   <router-link ><button class="btn">Guest Sign In</button></router-link>
    <router-link ><button class="btn">Sign Out</button></router-link>
    
    </div>
    <ul>
      <!-- <input v-model="message" placeholder="Name">
        <p>Name: {{ message }}</p>
        <input v-model="message" placeholder="Email">
        <p>Email: {{ message }}</p>
        <input v-model="message" placeholder="Phone">
        <p>Phone: {{ message }}</p>
        <input v-model="message" placeholder="Host's Name">
        <p> Looking for: {{ message }}</p> -->
    </ul>
    
    <h3>Essential Notices !!!</h3>
    <typical
  :steps="['Hello', 1000, 'Hello world!', 500]"
  :wrapper="'h2'"
></typical>
<typical
  class="typicalWrapper"
  :steps="['Hi', 1000, 'Awesome to see!', 500, 'Awesome to see you! Aha :-) 👋', 1000]"
  :loop="3"
  :wrapper="'h3'"
></typical>

    <!-- <img src="src\assets\handwash.gif" alt /> -->
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <div id="clock">
    <p class="date">{{ date }}</p>
    <p class="timer">{{ time }}</p>
    <p class="text">DIGITAL CLOCK with Vue.js</p>
</div>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul>
  </div>
</template>
<script src="https://cdn.jsdelivr.net/npm/vue-typical@latest/dist/typical.umd.min.js"></script>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
html,body {
    height: 100%;
}
body {
    background: #0f3854;
    background: radial-gradient(ellipse at center,  #0a2e38  0%, #000000 70%);
    background-size: 100%;
}
p {
    margin: 0;
    padding: 0;
}
#clock {
    font-family: 'Share Tech Mono', monospace;
    color: #ffffff;
    text-align: center;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    color: #daf6ff;
    text-shadow: 0 0 20px rgba(10, 175, 230, 1),  0 0 20px rgba(10, 175, 230, 0);}
    .timer {
        letter-spacing: 0.05em;
        font-size: 80px;
        padding: 5px 0;
    }
    .date {
        letter-spacing: 0.1em;
        font-size: 24px;
    }
    .text {
        letter-spacing: 0.1em;
        font-size: 12px;
        padding: 20px 0 0;
    }


h3 {
  margin: 20px 0 0;
  padding-top: 25px;
  padding-bottom: 30px;
  font-size: 25px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
  font-weight: bold;
}
a {
  color: red;
}

.btn {
  display: inline-block;
  padding: 0.8rem 6rem;
  text-decoration: none;
  font: inherit;
  font-size: 20px;
  font-weight: bold;
  border: 2.5px solid  #690009;;
  color:  #a7082f;
  background: rgb(245, 213, 176);
  border-radius: 40px 5px; 
  cursor: pointer;
  outline: none; 
}

.btn:hover,
.btn:active {
  background-color:  #ffa33b;
  color: rgb(252, 250, 180);
}

.btn.danger {
  color: red;
  border-color: red;
}

.btn.danger:hover,
.btn.danger:active {
  background: red;
  color: rgb(255, 255, 255);
}
.button {
   display: flex;
   padding: 0 10px;
   margin: 0 20px;
   justify-content: space-between;
}

.welcome-msg {
  position: relative;
  font-family: sans-serif;
  text-transform:capitalize;
  font-size: 2em;
  font-style: italic;
  letter-spacing: 4px;
  overflow: hidden;
  background: linear-gradient(90deg, rgb(233, 31, 31), rgb(243, 189, 10), rgb(253, 62, 62));
  background-repeat: no-repeat;
  background-size: 80%;
  animation: animate 2s linear infinite;
  -webkit-background-clip:text;
  -webkit-text-fill-color: rgba(197, 48, 73, 0);
}

@keyframes animate {
  0% {
    background-position: -500%;
  }
  100% {
    background-position: 500%;
  }
}


.tag-header{
  padding: 0 80px;
}

.blinking{
	animation:blinkingText 1.30s infinite;
  font-size: 20px;
padding-left: 200px;
padding-top: 30px;
text-align: center;
color:  rgb(201, 9, 57) ;
}
@keyframes blinkingText{
	25%{		color: rgb(247, 143, 73);	}
	49%{	color: transparent;	}
	50%{	color: transparent;	}
	99%{	color:transparent;	}
	100%{	color: rgb(233, 7, 7);	}
  
}
#blink-flash{
  text-align: center;
  align-content: center;
 padding-top: 200px; 
}

.typicalWrapper::after {
  content: "Please Wash Your Hands and Sanitize!!!";
  animation: blink 1s infinite step-start;
}

@keyframes blink {
  50% { opacity: 0; }
}
</style>
