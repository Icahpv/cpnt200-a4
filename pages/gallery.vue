<template>
  <v-container>
    <Header :headerPage="info" />
      <v-main>
        <Gallery v-for="content in contents" :key="content.id" :galleryPage="content" />
      </v-main>
    <Footer :footerPage="info" />
  </v-container>
</template>
<script>
export default {
  data () {
    return {
      info: {
        title: 'Nuxt-Travel',
        description: 'Where to travel nuxt?',
        author: 'Icah Vega',
        license: 'MIT License'
      },
      contents: [
        {
          location: 'Highland, United Kingdom',
          photographer: 'Gabriela Palai',
          account: 'https://www.pexels.com/@gabriela-palai-129458',
          image: 'images/uk.jpg',
          description: 'Famous train track from the film Harry Potter.',
          title: 'Train Track in Harry Potter'
        },
        {
          location: 'Machu Pichu, Peru',
          photographer: 'Errin Casano',
          account: 'https://www.pexels.com/@errin-casano-1240439',
          image: 'images/peru.jpg',
          description: 'Foggy view from the top of Machu Pichu.',
          title: 'Top View of Machu Pichu'
        },
        {
          location: 'Amsterdam, Nethderlands',
          photographer: 'Pierre Blaché',
          account: 'https://www.pexels.com/@pierre-blache-651604',
          image: 'images/canal.jpg',
          description: 'Romantic canal in Europe.',
          title: 'Canal in Amsterdam'
        },
        {
          location: 'French Polynesia',
          photographer: 'Julius Silver',
          account: 'https://www.pexels.com/@julius-silver-240301',
          image: 'images/french-polynesia.jpg',
          description: 'Beach with mountains',
          title: 'Beautiful beach with mountains'
        }
      ]
    }
  }
}
</script>
