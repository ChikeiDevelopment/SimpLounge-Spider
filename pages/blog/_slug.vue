<template>
  <article class="page-background">

    <div class="page-wrapper">

      <div class="header">
        <img :src="require(`~/assets/resources/${article.img}`)" alt="" class="img-design" />
      </div>

      <div class="article-content">
        <h1>{{ article.title }}</h1>
        <nuxt-content :document="article" />
      </div>

    </div>

  </article>
</template>

<script>
export default {
	async asyncData({ $content, params }) {
		const article = await $content('blog', params.slug).fetch();
		return { article }
	}
}
</script>

<style>
body {
  background-color: #0c0c0c;
  color: #aeaeae;
}

code[class*="language-"], pre[class*="language-"] {
  color: #fff
}

.page-wrapper {
  margin: auto;
  max-width: 1000px;
}

.header img {
  width: 100%;
  border-radius: 5px;
}

.page-background {
  background: url("assets/resources/web-design/blog-page-background.png") bottom no-repeat;
  background-size: cover;
  height: 89vh;
  min-height: 600px;
}

.img-design {
  border: .5px solid #ffffff30;
}

article {
  display: block;
  margin: 0 auto;
  padding: 50px 30px;
  max-width: 100%;
}

.article-content {
  margin: auto;
  max-width: 900px;
}

.page-wrapper h1 {
  font-size: 32px;
}

.page-wrapper h2 {
  font-size: 28px;
}

.page-wrapper h3 {
  font-size: 24px;
}

.page-wrapper h4 {
  font-size: 22px;
}

.page-wrapper h5 {
  font-size: 22px;
}

.page-wrapper h1, .page-wrapper h2, .page-wrapper h3, .page-wrapper h4, .page-wrapper h5 {
  padding-bottom: 10px;
  color: #fff;
  font-weight: 700;
}

</style>