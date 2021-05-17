<template>
  <header>
      <div class="title">My Website</div>
      <nav>
          <nuxt-link to="/">home</nuxt-link>
		  <nuxt-link to="/blogs">Blogs</nuxt-link>
		  <nuxt-link to="/rules">Rules</nuxt-link>
      </nav>
  </header>
</template>

<script>
export default {
	tansition: 'page'
	
}
</script>

<style>
header {
	padding: 15px 30px;
	background-color: rgb(37, 37, 37);
	display: flex;
	justify-content: space-between;
	align-items: center;
	box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.1);
}
header .title {
	color: #d8d8d8;
	font-size: 24px;
	font-weight: 900;
	text-transform: uppercase;
}
nav {
	display: flex;
	align-items: center;
	margin: 0 -15px;
}
nav a {
	display: block;
	margin: 0 15px;
	color: #9f25cf;
}
</style>