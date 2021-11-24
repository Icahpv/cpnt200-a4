<template>
  <v-container class="flex justify-center align-center text-left m-20">
    <v-main class=" flex justify-center align-center flex-col m-20">
       <h1 class="font-bold italic">"{{ galleryPage.title }}"</h1>
    <ul>
      <li>Photographer: {{ galleryPage.photographer }}</li>
      <li>Location: {{ galleryPage.location }} </li>
    </ul>
    </v-main>
       <nuxt-img class="max-w-screen-md mx-10" v-if="galleryPage.image" :src="galleryPage.image"  sizes="sm:50vw md:300px lg:758px" />
  </v-container>
</template>

<script>
export default {
  props: ['galleryPage']
}
</script>
