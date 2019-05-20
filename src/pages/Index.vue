<template>
  <Layout>
    
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->

    <div class="content">
      <g-image alt="PARABOLA" src="~/assets/img/logo-web-large.png" class="logo" />
      <h1>Site Coming Fall 2019</h1>

      <a href="https://thought-reactor.net">
        <g-image alt="Thought Reactor" src="~/assets/img/tr-logo.png" class="tr-logo" />
      </a>
    </div>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Site Coming Fall 2019'
  }
}
</script>

<style>
  img {
    width: 100%;
  }

  .logo {
    max-width: 900px;
  }

  div.content {
    text-align: center;
    padding: 2em;
  }

  .tr-logo {
    max-width: 320px;
    margin-top: 3em;
  }
</style>
