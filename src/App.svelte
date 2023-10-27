<script lang="ts">
  import About from "./components/About.svelte";
  import Videos from "./components/Videos.svelte";
  import Footer from "./components/Footer.svelte";
  let Y: number;
</script>

<main>
  <h1 id="header" class:scrolled={Y > 20}>STAR BACARY</h1>
  <p class="spacer" />
  <video src="/clip.mp4" autoplay muted loop />
  <Videos />
  <About />
  <Footer />
</main>

<svelte:window bind:scrollY={Y} />

<style lang="scss">
  @use "colors";

  main {
    overflow: hidden;
  }

  #header {
    position: fixed;
    top: 0;
    width: 100vw;
    z-index: 2;
    padding: 10px;
    font-family: Libel;
    font-size: 6em;
    margin: 20px;
    text-align: center;
    margin: 0;
    transition: all 0.4s;
    color: colors.$background_color;
    background-color: colors.$background_color_dark;
    &.scrolled {
      font-size: 3em;
      letter-spacing: 20px;
    }
  }

  p.spacer {
    height: 140px;
    margin: 0;
    background-color: colors.$background_color_dark;
  }

  video {
    display: block;
    width: 100%;
    background-color: colors.$background_color_dark;
  }

  @media (max-width: 800px) {
    #header {
      font-size: 4em;
      &.scrolled {
        font-size: 2em;
      }
    }
    video {
      width: 200%;
      position: relative;
      left: -45%;
      overflow-y: hidden;
    }
  }
</style>
