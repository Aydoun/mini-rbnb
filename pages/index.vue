<template>
  <div class="container">
    <Header />
    <div>
      <h1 class="title">
        minirbnb
      </h1>
    </div>
    <div>
      <NLink to="/about">
        about page
      </NLink>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue';
import Header from '~/components/Header.vue';

export default {
  components: {
    Logo,
    Header,
  }
}
</script>

<style>
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
