<template>
  <Layout>
    <div class="content">
      <div class="logo-container">
        <div class="logos">
          <g-image alt="PARABOLA" src="~/assets/img/logo_white.svg" class="logo bottom" />
          <g-image alt="PARABOLA" src="~/assets/img/logo_white.svg" class="logo middle" />
          <g-image alt="PARABOLA" src="~/assets/img/logo_white.svg" class="logo top" />
        </div>

        <h1>A Physics-driven First Person Puzzle Game</h1>
        <h2>Official Site Coming Holiday 2019</h2>

        <a href="https://thought-reactor.net">
          <g-image alt="Thought Reactor" src="~/assets/img/tr-logo.png" class="tr-logo" />
        </a>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Site Coming Holiday 2019"
  }
};
</script>

<style lang="scss">
div.content {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
}

div.logo-container {
  position: absolute;
  width: 85%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  div.logos {
    margin-bottom: 12.5%;
    display: flex;
    justify-content: center;

    .logo {
      max-width: 1280px;
      position: absolute;
      top: 0;

      &.middle {
        opacity: 0.5;
        animation: logoJitter 1500ms infinite;
        transform: skewX(0) translateX(0);
      }

      &.bottom {
        animation: logoPulse 5s infinite;
      }
    }
  }

  h1 {
    color: #666;
  }

  h2 {
    color: #444;
  }
}

@keyframes logoPulse {
  0% {
    filter: drop-shadow(0 0 10px rgba(255, 255, 255, 0.45));
  }
  50% {
    filter: drop-shadow(0 0 15px rgba(255, 255, 255, 0.85));
  }
  100% {
    filter: drop-shadow(0 0 10px rgba(255, 255, 255, 0.45));
  }
}

@keyframes logoJitter {
  0% {
    transform: skewX(2deg) translateX(-2px);
  }
  25% {
    transform: skewX(0) translateX(0);
  }
  50% {
    transform: skewX(-2deg) translateX(2px);
  }
  75% {
    transform: skewX(2deg) translateX(-2px);
  }
  100% {
    transform: skewX(0) translateX(0);
  }
}

a {
  opacity: 0.6;
  filter: grayscale(1);
  transition: all 200ms ease-in-out;

  &:hover {
    opacity: 1;
    filter: grayscale(0);
  }

  .tr-logo {
    max-width: 240px;
    margin-top: 12.5%;
  }
}
</style>
