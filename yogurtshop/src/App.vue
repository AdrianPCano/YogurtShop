<template>
  <v-app>
    <v-toolbar app class="grey lighten-2" flat height = "120">
      <v-toolbar-title class="headline text-uppercase">
      </v-toolbar-title>
      <v-image v-for="image in image" :key="image.image">
      <img :src="image.image"></img>
      </v-image>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>


export default {
  name: 'App',
  data () {
    return {
      image: [
        {image:"/logo.png"}
      ]
    }
  }
}
</script>
