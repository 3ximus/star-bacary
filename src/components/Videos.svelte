<div class="videos">
  <h1>Vidéos</h1>

  <div class="list">
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/PcSIhzh00S4?si=eWMr1dIfgT7ti09j"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen
    />
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/MqA2AAAtwOw?si=w5NrybFDQKl1KlTV"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen
    />
    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/7rv8Jjn0M-c?si=rvBXtRvo8NauBLLW"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen
    />
  </div>

  <div class="more">
    <a href="https://youtube.com/@bacarysonko4852">
      Plus de Vidéos&nbsp&nbsp
      <svg width="40" height="40" viewBox="0 0 50 50">
        <path
          d="M 44.898438 14.5 C 44.5 12.300781 42.601563 10.699219 40.398438 10.199219 C 37.101563 9.5 31 9 24.398438 9 C 17.800781 9 11.601563 9.5 8.300781 10.199219 C 6.101563 10.699219 4.199219 12.199219 3.800781 14.5 C 3.398438 17 3 20.5 3 25 C 3 29.5 3.398438 33 3.898438 35.5 C 4.300781 37.699219 6.199219 39.300781 8.398438 39.800781 C 11.898438 40.5 17.898438 41 24.5 41 C 31.101563 41 37.101563 40.5 40.601563 39.800781 C 42.800781 39.300781 44.699219 37.800781 45.101563 35.5 C 45.5 33 46 29.398438 46.101563 25 C 45.898438 20.5 45.398438 17 44.898438 14.5 Z M 19 32 L 19 18 L 31.199219 25 Z"
        />
      </svg>
    </a>
  </div>
</div>

<style lang="scss">
  @use "../colors";

  div.videos {
    background-color: colors.$background_color_dark;
    color: colors.$background_color;
    h1 {
      font-family: Libel;
      font-size: 4em;
      letter-spacing: 4px;
      text-align: center;
      margin-top: 0px;
      padding-top: 60px;
    }

    .list {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-wrap: wrap;
      gap: 60px;
      padding-top: 30px;
      padding-bottom: 50px;
    }
  }
  div.more {
    fill: colors.$background_color;
    display: flex;
    justify-content: center;
    font-size: 1.5em;
    padding-bottom: 50px;
    a {
      display: flex;
      align-items: center;
      color: colors.$background_color;
      font-family: Libel;
      letter-spacing: 2px;
      text-decoration: none;
      transition: all 0.4s;
      cursor: pointer;
      &:hover {
        scale: 1.1;
      }
    }
  }
  @media (max-width: 800px) {
    div.videos {
      h1 {
        font-size: 3em;
      }
      .list {
        flex-direction: column;
        iframe {
          max-width: 90%;
        }
      }
    }
  }
</style>
