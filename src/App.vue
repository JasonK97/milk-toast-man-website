<template>
  <div id="app">
    <app-header />
    <music-player />
    <router-view />
    <app-footer />
  </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
import AppFooter from '@/components/AppFooter.vue'
import MusicPlayer from '@/components/MusicPlayer.vue'

export default {
  components: {
    AppHeader,
    AppFooter,
    MusicPlayer
  },
  data () {
    return {}
  }
}
</script>

<style>
#nav {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}

#nav a:hover {
  color: #6e6e6e;
}

#nav a.router-link-exact-active {
  color: #34c2db;
}

#headerLogo {
    border: 3px solid black;
    border-radius: 50%;
    height: 150px;
    display: inline-block;
    margin-left: 45.5%;
    margin-right: 50%;
}

.musicPlayer {
  position: -webkit-sticky;
  position: sticky;
  top: 250px;
  transition: 1s transform cubic-bezier(0,.12,.14,1);
  z-index: 3;
}

.slider {
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
  border: 3px solid gray;
  border-left: none;
  background-color: white;
  padding: 10px 0px 10px 30px;
  width: 70px;
  margin-right: 97vw;
  margin-top: -15vh;
  cursor: pointer;
}

.bandcamp {
  border: 2px solid gray;
  width: 350px;
  height: 786px;
  z-index: 4;
  margin-top: -150px;
  margin-left: -34vw;
}

.open {
  transform: translateX(360px);
}

.parallaxPic {
    min-height: 600px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.parallaxPic {
    background-image: url("./assets/Derek Desk.jpg");
    min-height: 450px;
}

.caption {
    position: absolute;
    left: 0;
    top: 50%;
    width: 100%;
    letter-spacing: 2px;
    /* -webkit-text-stroke: 1px rgb(199, 198, 198); */
}

.caption span.title {
    color: rgb(255, 255, 255);
    padding: 15px;
    font-size: 60px;
    font-family: 'Overpass', sans-serif;
    text-align: left;
    margin-left: 150px;
    text-shadow: 6px 4px 3px rgb(24, 24, 24);
}

.caption span.sub-title {
    color: rgb(255, 255, 255);
    padding: 15px;
    font-size: 25px;
    font-family: 'Overpass', sans-serif;
    text-align: left;
    margin-left: 150px;
    text-shadow: 4px 3px 3px rgb(24, 24, 24);
}

#quote {
    margin: 25px 10px 25px 10px;
}

#quotePic {
    float: left;
    height: 600px;
    overflow: auto;
}

#quoteText {
    font-size: 32px;
    background-color: rgb(172, 242, 255);
    padding-top: 220px;
    padding-bottom: 220px;
    font-family: 'Didact Gothic', sans-serif;
    text-shadow: 5px 5px 10px rgb(75, 75, 75);
}

#quoteText p {
  text-align: center;
}

#video {
    position: relative;
    height: 0;
    padding-bottom: 50%;
    overflow: hidden;
}

iframe {
    width: 75%;
    height: 75%;
    position: absolute;
    top: 10%;
    left: 15%;
}

#contactStuff {
    background-image: url("./assets/Evergreen Blues.jpg");
    padding: 25px 0px 25px 0px;
    background-position: center;
    background-repeat: no-repeat;
    margin-bottom: 50px;
}

#contactInfo {
    text-align: center;
    background-color: rgb(172, 242, 255);
    margin: 50px 200px 50px 200px;
    font-family: 'Overpass', sans-serif;
    font-size: 24px;
    padding: 50px 25px 50px 25px;
    border-radius: 10px;
    border: 3px solid gray;
}

/* .about {
    background-image: url('./assets/Empty-Sky.jpg');
    background-repeat: no-repeat;
    padding: 25px 0px 0px 0px;
    margin: 0px 5% 25px 7%;
    width: 100%;
} */

#aboutPic {
    float: right;
    height: 590px;
    overflow: auto;
    border-radius: 10px;
    border: 3px solid gray;
    margin: 0px 300px 50px 0px;
}

#aboutBox {
    margin: 25px 52% 25px 300px;
    border: 3px solid gray;
    border-radius: 10px;
}

#about-text {
    font-size: 20px;
    background-color: rgb(172, 242, 255);
    padding: 50px 100px 50px 50px;
    font-family: 'Didact Gothic', sans-serif;
    border-radius: 10px;
    /* text-shadow: 5px 5px 10px rgb(75, 75, 75); */
}

.about {
    font-size: 20px;
}

#contactBtn {
    text-decoration: none;
    background-color: rgb(15, 15, 29);
    color: whitesmoke;
    font-size: 20px;
    padding: 5px 5px 5px 5px;
    border-radius: 3px;
    border: 1px solid gray;
}

.inputAreas {
    font-family: 'Overpass', sans-serif;
    padding: 10px 5px 10px 5px;
    border-radius: 5px;
    border: 2px solid gray;
    size: 50;
}

.btns {
    font-family: 'Overpass', sans-serif;
    font-size: 18px;
    padding: 10px 20px 10px 20px;
    border-radius: 5px;
    border: 2px solid black;
    background-color: black;
    color: whitesmoke;
}

.btns:hover {
    border: 2px solid gray;
    background-color: whitesmoke;
    color: black;
    cursor: pointer;
}

.musicPlayer {
    text-align: center;
    display: flex;
    justify-content: center;
}

#footer {
    text-align: center;
}

#footerText {
    text-decoration: none;
    font-family: 'Overpass', sans-serif;
    color: black;
}

/*******************Higher Resolution Screens*******************/

/* @media screen and (min-width: 1800px) {
    .parallaxPic {
        min-height: 450px;
    }
    .caption {
        top: 50%;
    }
    #quotePic {
        float: left;
        height: 600px;
        overflow: auto;
    }
    #quoteText {
        padding: 150px 100px 320px 1000px;
    }
    #aboutPic {
        float: right;
        height: 845px;
        overflow: auto;
        margin-right: 25px;
    }
    #aboutBox {
        margin: 25px 50% 25px 10px;
    }
    #about {
        font-size: 32px;
        background-color: rgb(172, 242, 255);
        padding: 50px 100px 50px 50px;
        font-family: 'Didact Gothic', sans-serif;
    }
} */

/*******************Mobile Devices*******************/

@media screen and (max-width: 800px) {
  #app {
    display: block;
    justify-content: center;
    width: 100%;
  }
  .bandcamp {
    margin-left: -112vw;
  }
  .parallaxPic {
      min-height: 275px;
      background-position: center top;
      background-repeat: no-repeat;
      background-size: cover;
      margin-left: 1vw;
      margin-right: -30vw;
  }
  .caption {
      top: 50%;
      text-align: center;
  }
  .caption span.title {
      padding: 10px;
      margin-left: 5px;
  }
  .caption span.sub-title {
      padding: 15px;
      margin-left: 10px;
  }
  #quotePic {
      float: left;
      width: 100%;
      overflow: auto;
  }
  #quoteText {
      padding: 350px 100px 100px 100px;
  }
  #contactInfo {
      margin: 50px 10px 50px 10px;
      padding: 10px 25px 10px 25px;
  }
  .inputAreas {
      size: 25;
  }
}
</style>
