<template>
  <div>
    <div v-for="article in articles" :key="article.id">
      <nuxt-link :to="`posty/${article.slug}`">{{ article.title }}</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',

  data: () => ({
    articles: [
      {
        id: 'article1',
        slug: 'wstep-do-nuxt-czesc-1',
        title: 'Wstep do nuxt czesc 1'
      },
      {
        id: 'article2',
        slug: 'wstep-do-nuxt-czesc-2',
        title: 'Wstep do nuxt czesc 2'
      }
    ]
  })
}
</script>
