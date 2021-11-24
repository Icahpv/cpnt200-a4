<template>
  <v-container class="flex justify-center align-center flex-col text-center p-10 bg-gray-200">
    <p class="text-xl text-gray-600">&copy; <NuxtLink to="https://github.com/Icahpv">{{ footerPage.author }}</NuxtLink> || {{ footerPage.license }}</p>
  </v-container>
</template>
<script>
export default {
  props: ['footerPage']
}
</script>
