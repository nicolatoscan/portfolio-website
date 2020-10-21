<template>
  <header>
    <h1>NICOLA TOSCAN</h1>
    <h2>SITE UNDER CONSTRUCTION</h2>
  </header>
  <main>
    <div id="about-me" class="main-section">
      <div class="main-container">
        <h2>About me</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
          nam quas, deserunt et rem qui quis repellat eveniet expedita
          repudiandae deleniti amet excepturi fugit necessitatibus quam
          aspernatur officia, voluptatum ex.
        </p>
      </div>
    </div>
    <div id="projects" class="main-section">
      <div class="main-container">
        <h2>Projects</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis
          nam quas, deserunt et rem qui quis repellat eveniet expedita
          repudiandae deleniti amet excepturi fugit necessitatibus quam
          aspernatur officia, voluptatum ex.
        </p>
      </div>
    </div>
  </main>
  <footer>
    <p>
      Nicola Toscan | <a href="https://github.com/nicolatoscan">GitHub</a> | <a href="https://www.linkedin.com/in/nicolatoscan/">LinkedIn</a>
    </p>
  </footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {
  },
});
</script>

<style lang="less">
body { margin: 0 !important; }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
  color: white;
  background-color: #222222;
  background: linear-gradient(-45deg, #0f2027, #203a43, #2c5364);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  cursor: default;
}
header {
  user-select: none;
  height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  h1,
  h2 {
    text-align: center;
    display: block;
  }
  h1 {
    letter-spacing: 0.7em;
    font-weight: 100;
    padding-left: 0.7em;
    border-left: 1px solid white;
    border-right: 1px solid white;
    margin: 15px 1em;
    display: inline-block;
    font-size: 4.5vw;
  }
  h2 {
    font-weight: 100;
    color: #aaa;
    letter-spacing: 0.4em;
    margin: 15px;
    display: inline-block;
    font-size: 2vw;
    margin-left: 2em;
    margin-right: 2em;
  }
}
main {
  margin: 0;
  padding: 0;
  width: 100wv;
  overflow: hidden;

  > .main-section {
    background-color: #222222;
    transform: rotate(1deg);
    width:110%;
    top:-5%;
    left:-5%;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 2em 0;

    > .main-container {
      padding: 1.5em 2em;
      margin: 0 5%;
      transform: rotate(-1deg);
      max-width: 960px;

      h2 {
        padding-left: 0.5em;
        border-left: 3px white solid;
      }
    }
  }
}
footer {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: flex-end;
  margin-top: 3em;
  > p {
    letter-spacing: 0.2em;
    margin: 1em;
  }
  a {
    text-decoration: none;
    color: white;
  }
}
@media screen and (min-width: 1600px) {
  h1 {
    font-size: 5em;
  }
  header > p {
    font-size: 2em;
  }
}
@media screen and (max-width: 800px) {
  h1 {
    font-size: 2.3em !important;
  }
  header > p {
    font-size: 1em;
  }
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

</style>
