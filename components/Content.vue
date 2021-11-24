<template>
  <v-container class="flex justify-center align-center flex-col text-center pt-20 m-auto">
    <h1 class="text-4xl p-5">{{ contentPage.quote }}</h1>
    <p class="text-2xl pb-10">- {{ contentPage.author }}</p>
  </v-container>
</template>
<script>
export default {
  props: ['contentPage']
}
</script>
