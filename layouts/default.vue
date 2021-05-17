<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  transiton: 'page'
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  font-family: sans-serif;
}

a {
  text-decoration: none;
}

p {
  margin-bottom: 15px;
}

p:last-of-type {
  margin-bottom: 0px;
}
</style>
