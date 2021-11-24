<template>
  <v-container class="flex justify-center align-center flex-col text-center p-10 bg-gray-200">
    <p>&copy; {{ footerPage.author }} || {{ footerPage.license }}</p>
  </v-container>
</template>
<script>
export default {
  props: ['footerPage']
}
</script>
