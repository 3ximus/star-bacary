<div class="videos">
  <h1>Videos</h1>

  <a href="https://youtube.com/@bacarysonko4852?si=oOifgrtjNjh2pESC">YOUTUBE</a>

  <div class="list">
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
      padding-top: 10px;
    }

    .list{
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10%;
    }
  }
</style>
