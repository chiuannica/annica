<template>
  <div id="app">
    <Scrollbar></Scrollbar>
    <div id="body">
      <Header></Header>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Scrollbar from './components/Scrollbar'
import Header from './components/Header'
import Home from './components/Home'
import About from './components/About'
import Projects from './components/Projects'
import Contact from './components/Contact'

export default {
  name: 'App',
  components: {
    Scrollbar, Header, Home, About, Projects, Contact
  }
}
</script>

<style>
@font-face {
  font-family: 'Catamaran';
  src: url('assets/Catamaran-Regular.ttf');
}
@font-face {
  font-family: 'DMSans';
  src: url('assets/DMSans-Regular.ttf');
}
@font-face {
  font-family: 'Varela';
  src: url('assets/VarelaRound-Regular.ttf');
}

@font-face {
  font-family: 'Anon';
  src: url('assets/AnonymousPro-Regular.ttf');
}

@font-face {
  font-family: 'Machina';
  src: url('assets/NeueMachina-Regular.otf');
}

@font-face {
  font-family: 'Machina-Bold';
  src: url('assets/NeueMachina-Ultrabold.otf');
}

#body {
  font-family: 'DMSans', 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  -webkit-font-smoothin: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: hsl(216, 21%, 13%);
  margin-left: 10%;
  margin-right: 10%;
  opacity: 1;
  width: 80%;
}
body {
  font-size: 62.5%;
  margin: 0;
  text-shadow: 0.01em 0.01em 0.01em hsl(216, 21%, 13%);
}
h1, h2, h3, h4, h5 {
  color: hsl(216, 21%, 13%);
  line-height: 0.8;
  padding: 0;
}
h1, h2, h3, a {
  font-family: 'Anon', 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
h1 {
  font-size: 3.2rem;
}
h2 {
  font-size: 3.0rem;
}
h3 {
  font-size: 2.4rem;
  font-style: none;
}
h4, h5 {
  font-size: 2.1rem;
  color: #ebc1c5cc;
}
h6 {
  font-size: 2.1rem;
  color: #354051;
  margin: 0;
}
p, li {
  font-size: 1.8rem;
  margin: 0 0;
  line-height: 1.2;
}
ul {
  margin: 0;
}
a {
  font-size: 2.1rem;
  line-height: 0.9;
  color: #354051;
  text-decoration: none;
  transition: color 0.7s;
}
@media screen and (max-width: 768px) {
  #body {
    margin-left: 2%;
    margin-right: 2%;
    width: 96%;
  }

  h1, h2, h3, h4, h5 {
    line-height: 1;
  }
  h1 {
  font-size: 2.6rem;
  }
  h2 {
    font-size: 2.0rem;
  }
  h3 {
    font-size: 1.8rem;
  }
  h4, h5 {
    font-size: 1.6rem;
  }
  h6 {
    font-size: 1.6rem;
  }
  p, li, a {
    font-size: 2.5em;
  }
}
</style>
