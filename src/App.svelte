<script lang="ts">
  import About from "./components/About.svelte";
  import Videos from "./components/Videos.svelte";

  let Y: number;
</script>

<main>
  <h1 id="header" class:scrolled={Y > 20}>STAR BACARY</h1>
  <p class="spacer" />
  <video src="/clip.mp4" autoplay muted loop />
  <About />
  <Videos />
</main>

<svelte:window bind:scrollY={Y} />

<style lang="scss">
  @use "colors";

  #header {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 2;
    padding: 10px;
    font-family: Libel;
    font-size: 6em;
    margin: 20px;
    text-align: center;
    margin: 0;
    transition: all 0.4s;
    color: colors.$color_dark;
    &.scrolled {
      font-size: 3em;
      letter-spacing: 20px;
      background-color: colors.$background_color;
    }
  }

  p.spacer {
    height: 125px;
  }

  video {
    width: 100%;
    opacity: 90%;
  }
</style>
