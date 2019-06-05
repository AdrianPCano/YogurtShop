<template>
  <div class = 'index'>
    <v-toolbar class="grey lighten-2" flat height = "120">
      <v-layout justify-space-around>
          <v-image v-for="image in image" :key="image.image">
            <img :src="image.logo">
          </v-image>
        <v-toolbar-title class="headline text-uppercase">
          <span class="mr-5">Home</span>
          <span class="mr-5">About</span>
          <span class="mr-5">Blog</span>
          <span class="mr-2">Contact</span>  
        </v-toolbar-title>
      </v-layout>
    </v-toolbar>
    <v-container>
      <v-layout>
        <v-image v-for="image in image" :key="image.image">
          <img :src="image.back">
        </v-image>
      </v-layout>
    </v-container>
    <div class="bottom" >
      <v-layout row> 
        <v-flex class="pb-5 grey lighten-2"> 
          <v-container >
            <h1 class="pt-3 pb-2 brown--text text--lighten-1">NEW PRODUCT</h1>
            <h2 class="pb-3  pink--text display-1">The Twist of Healthy Yogurt</h2>
            <p class="body-1">This website template has been designed by freewebsitetemplates.com for you, for free. You can replace all this text with your own text.</p>
            <v-spacer></v-spacer>
            <v-layout justify-space-between>
            <v-image height="100" v-for="image in image" :key="image.image">
              <img :src="image.yogurt">
            </v-image>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <div class="bottom" >
      <v-layout row>
        <v-flex class="pb-5 blue" > 
          <v-container>
            <h1>NEW PRODUCT</h1>
            <h2 class="pink--text">The Twist of Healthy Yogurt</h2>
            <p>This website template has been designed by freewebsitetemplates.com for you, for free. You can replace all this text with your own text.</p>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      image: [
        {logo:"/logo.png"},
        {back:"/bg-home.jpg"},
        {yogurt:"/yogurt.jpg"}
      ]
    }
  }
}
</script>

