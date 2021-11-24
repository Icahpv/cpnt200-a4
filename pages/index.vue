<template>
  <v-container>
    <Header :headerPage="info" />
    <h1 class="text-7xl p-10 text-center"> Inspirational Travel quotes </h1>
    <Content v-for="quote in quotes" :key="quote.id" :contentPage="quote" />
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
          image: 'uk.jpg'
        },
        {
          location: 'Machu Pichu, Peru',
          photographer: 'Errin Casano',
          account: 'https://www.pexels.com/@errin-casano-1240439',
          image: 'peru.jpg'
        },
        {
          location: 'Canal, Europe',
          photographer: 'Pierre Blaché',
          account: 'https://www.pexels.com/@pierre-blache-651604',
          image: 'canal.jpg'
        },
        {
          location: 'French Polynesia',
          photographer: 'Julius Silver',
          account: 'https://www.pexels.com/@julius-silver-240301',
          image: 'french-polynesia.jpg'
        }
      ],
      quotes: [
        {
          quote: '“A journey of a thousand miles begins with a single step”',
          author: 'Lao Tzu'
        },
        {
          quote: '"“Do not follow where the path may lead. Go instead where there is no path and leave a trail”',
          author: 'Ralph Waldo Emerson'
        },
        {
          quote: '“I am not the same, having seen the moon shine on the other side of the world”',
          author: 'Mary Anne Radmacher'
        },
        {
          quote: '“Man cannot discover new oceans unless he has the courage to lose sight of the shore” ',
          author: 'Andre Gide'
        },
        {
          quote: '“We take photos as a return ticket to a moment otherwise gone”',
          author: 'Katie Thurmes'
        },
        {
          quote: '“There’s a sunrise and a sunset every single day, and they’re absolutely free. Don’t miss so many of them”',
          author: 'Jo Walton'
        }
      ]
    }
  }
}
</script>
