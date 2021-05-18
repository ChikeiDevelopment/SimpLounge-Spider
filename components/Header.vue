<template>
  <header>
    <nav class="nav">
      <div class="container centered">
        <ul class="navigation">
          <li class="content">
            <nuxt-link to="/" class="button home">Home</nuxt-link>
          </li>
          <li class="content">
            <nuxt-link to="/rules" class="button rules">Rules</nuxt-link>
          </li>
          <li class="content">
            <font-awesome-icon :icon="['fas', 'star']" class="scaling"/>
          </li>
          <li class="content">
            <nuxt-link to="/blogs" class="button blog">Blog</nuxt-link>
          </li>
          <li class="content">
            <nuxt-link to="/" class="button store">Store</nuxt-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  tansition: "page",
};
</script>

<style>

.nav {
  margin-top: 1.5rem;
  margin-bottom: 0.5rem;
}

.container {
  max-width: 1100px;
}

.centered {
  margin-left: auto;
  margin-right: auto;
}

.navigation {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 -0.75rem 0.75rem -0.75rem;
  letter-spacing: 0.1em;
  list-style: none;
  text-transform: uppercase;
  font-weight: 700;
  text-shadow: rgba(0, 0, 0, 0.3) 0 2px 0;
  font-size: 1.125rem;
}

.content {
  margin: 0 0.75rem 0 0.75rem;
}

.content a.button {
  display: flex;
  align-items: center;
  padding: 0.55rem 1.25rem 0.55rem 1.25rem;
  border: 1px solid hsla(0, 0%, 100%, 0.3);
  color: #fff;
  border-radius: 2px;
}

.content a.button.home {
  background-color: #ffbc49;
  border-bottom: 4px solid #bd8f42;
}

.content a.button.home:hover {

}

.content a.button.rules {
  background-color: #28c188;
  border-bottom: 4px solid #1e8e65;
}

.content a.button.blog {
  background-color: #37c4b4;
  border-bottom: 4px solid #228e82;
}

.content a.button.store {
  background-color: #f70174;
  border-bottom: 4px solid #95114e;
}
</style>