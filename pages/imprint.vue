<template>
  <div class="container">
    <div>
      <h1>Imprint</h1>
      <div>
        <p>Responsible for content in accordance with 55 Abs. 2 RStV</p>
        <p>
          Mario Kaiser<br />
          Graudenzer Str. 17<br />10243 Berlin
        </p>
        <p>Contact me at ehmprah@gmail.com</p>
      </div>
      <a href="/">Back</a>
    </div>
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue';

export default {
  // components: {
  //   Logo
  // }
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: #222;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
