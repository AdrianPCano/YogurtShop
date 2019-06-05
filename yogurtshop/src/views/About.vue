<template>
  <div class="about">
    <v-toolbar class="grey lighten-2" flat height = "120">
      <v-layout justify-space-around>
          <v-image v-for="image in image" :key="image.image">
            <img :src="image.logo">
          </v-image>
      </v-layout>
      <v-layout justify-space-around>
        <v-toolbar-title class="headline text-uppercase">
          <span class="mr-5">Home</span>
          <span class="mr-5">About</span>
          <span class="mr-5">Blog</span>
          <span class="mr-2">Contact</span>  
        </v-toolbar-title>
      </v-layout>
    </v-toolbar>
    <v-container class="my-5">
    </v-container>
  </div>
</template>

<script>
export default {
  data () {
    return {
      image: [
        {logo:"/logo.png"}
      ]
    }
  }
}
</script>