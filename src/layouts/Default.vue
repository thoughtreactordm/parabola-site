<template>
  <div class="layout">
    <!--<header class="header">
      <strong>
        <g-link to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about">About</g-link>
      </nav>
    </header>-->
    <slot />
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Lato:400,900|Montserrat+Alternates:200,400&display=swap");

html,
body {
  height: 100vh;
}

body {
  background: black;
  color: white;
  height: 100%;

  padding: 0;
  margin: 0;
  font-family: "Lato", sans-serif;

  h1,
  h2,
  h3 {
    font-family: "Montserrat Alternates", sans-serif;
    font-weight: 200;
  }

  img {
    width: 100%;
  }
}
</style>
