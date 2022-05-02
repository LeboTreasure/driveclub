<template>
  <div id="app">
    <nav>
      <img class="logo" src="./assets/logo.svg" />
      <router-link to="/">HOME</router-link>
      <router-link to="/contact">CONTACT US</router-link>
    </nav>

    <router-view />

    <footer>
      <div class="content">
        <img class="logo" src="./assets/logo.svg" /> <br />
        <div class="icons">
          <img src="./assets/facebook.svg" />
          <img src="./assets/instagram.svg" />
          <img src="./assets/twitter.svg" />
          <img src="./assets/linkedin.svg" />
          <img src="./assets/youtube.svg" />
        </div>
        <div class="links">
          <div class="models">
            <h3>MODELS</h3>
            <router-link to="/learn">LA FERRARI</router-link><br />
            <router-link to="/learn">MODEL S</router-link>
          </div>

          <div class="more">
            <h3>MORE</h3>
            <router-link to="/">HOME</router-link><br>
            <router-link to="/contact">CONTACT</router-link>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
#app {
  background-image: url("./assets/hero-home.jpg");
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
}

nav {
  padding: 30px;

  .logo {
    display: flex;
    flex-direction: row;
    padding-left: 10%;
  }

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
footer {
  .logo {
    display: flex;
    flex-direction: row;
    padding-left: 5%;
  }
  .content {
    align-content: left;
    padding-left: 10%;
  }
  .icons {
    display: flex;
    flex-direction: row;
    padding-left: 5%;
  }
  .models {
    padding-right: 20px;
  }
  .more {
    padding-right: 10px;
  }
  .links {
    .models {
      padding-left: 20%;
      display: flex;
      flex-direction: row;
    }
    .more {
      padding-left: 60%;
      display: flex;
      flex-direction: row;
    }
  }
}
</style>
