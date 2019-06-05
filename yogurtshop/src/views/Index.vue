<template>
  <div class = 'index'>
    <v-toolbar class="grey lighten-2" flat height = "120">
      <v-layout justify-space-around>
          <v-img v-for="image in image" :key="image.image">
            <img :src="image.logo">
          </v-img>
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
        <v-img v-for="image in image" :key="image.image">
          <img :src="image.back">
        </v-img>
      </v-layout>
    </v-container>
    <div>
      <v-layout row> 
        <v-flex class="pb-5 grey lighten-2"> 
          <v-container >
            <h1 class="pt-3 pb-2 title brown--text text--lighten-1">NEW PRODUCT</h1>
            <h1 class="pb-3 change-font pink--text">The Twist of Healthy Yogurt</h1>
            <p class="body-1">This website template has been designed by freewebsitetemplates.com for you, for free. You can replace all this text with your own text.</p>
            <v-spacer></v-spacer>
            <v-layout justify-space-between>
            <v-img v-for="image in image" :key="image.image">
              <img :src="image.yogurt">
            </v-img>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <div>
      <v-layout row>
        <v-flex class="pb-5 lime darken-1 " > 
          <v-container>
            <h1>NEW PRODUCT</h1>
            <h2 class=" pink--text">The Twist of Healthy Yogurt</h2>
            <p>This website template has been designed by freewebsitetemplates.com for you, for free. You can replace all this text with your own text.</p>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <v-footer >
      <v-layout row>
        <v-flex class="pink" > 
          <v-container back>
              <a href="" class="display-a"></a>
							<h1>PRODUCTS</h1>
          </v-container>
        </v-flex>
      </v-layout>
    </v-footer>
  </div>
</template>


<style lang="stylus" scoped>
.change-font {
    font-family: "Magra-bold", Sans, serif;
    font-weight: 900;
}
</style>

<style lang="stylus">
.back {
  background: url(/icons.png) no-repeat;
	display: block;
	height: 44;
	margin: 0 auto 22px;
	padding: 0;
	width: 80px;
}
</style>

<style lang="stylus" scoped>
.display-a {
    background-position: 0 -372px;
}
</style>

<style lang="stylus" scoped>
.display-b {
    font-family: "Magra-bold", Sans, serif;
    font-weight: 900;
}
</style>

<style lang="stylus" scoped>
.display-c {
    font-family: "Magra-bold", Sans, serif;
    font-weight: 900;
}
</style>

<style lang="stylus" scoped>
.display-d {
    font-family: "Magra-bold", Sans, serif;
    font-weight: 900;
}
</style>


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

