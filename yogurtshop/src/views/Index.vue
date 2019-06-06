<template>
  <div class = 'index'>
    <v-toolbar class="grey lighten-2" flat height = "120">
      <v-layout justify-space-around>
        <router-link to="/">
          <v-img v-for="image in image" :key="image.image">
            <img :src="image.logo">
          </v-img>
        </router-link>
      </v-layout>
      <v-layout justify-space-around>
        <v-toolbar-title class="headline text-uppercase">
          <span class="mr-5 fontTool">Home</span>
          <span class="mr-5 fontTool">About</span>
          <span class="mr-5 fontTool" >Blog</span>
          <router-link to="About">
            <span class="mr-2 fontTool">Contact</span> 
          </router-link> 
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
      <v-layout row wrap> 
        <v-flex class="backCol"> 
          <v-container >
            <h1 class=" mt-2 title brown--text text--lighten-1">NEW PRODUCT</h1>
            <h1 class=" mt-2 change-font pink--text">The Twist of Healthy Yogurt</h1>
            <p class=" maxWid body-1">This website template has been designed by freewebsitetemplates.com for you, for free. You can replace all this text with your own text.</p>
            <v-spacer></v-spacer>
            <v-layout class="imageSth" justify-space-between>
            <v-img v-for="image in image" :key="image.image">
              <img :src="image.yogurt">
            </v-img>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <div>
      <v-layout row class="blockDis">
        <v-flex class="lime darken-1 " > 
          <v-container >
            <router-link to="About">
							<v-avatar class="blockIcons">
                <img src="/yogu.png"> 
							</v-avatar>
              <v-avatar class=" blockIcons">
                <img src="/story.jpg">
              </v-avatar>
              <v-avatar class="blockIcons">
                <img src="/flavor.png"> 
              </v-avatar>
              <v-avatar class="blockIcons">
                <img src="/location.png">
              </v-avatar>
            </router-link>
          </v-container>
        </v-flex>
      </v-layout>
      <v-layout row wrap class="blockDis">
        <v-flex class="lime darken-1" > 
          <v-container  class="white--text ">
            <h1 class="iconText00"> PRODUCTS</h1>
            <h1 class="iconText11"> OUR STORY</h1>
            <h1 class="iconText22"> FLAVORS</h1>
            <h1 class="iconText33"> OUR LOCATION</h1>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <v-footer  class="blockDis footerWid" >
      <v-layout row>
        <v-flex class="pink" > 
          <v-container>
            <router-link to="/">
							<v-avatar class="mr-5">
                <img src="/facebook.jpg"> 
							</v-avatar>
              <v-avatar class="mr-5">
                <img src="/twitter.png">
              </v-avatar>
              <v-avatar class="mr-5">
                <img src="/google.png"> 
              </v-avatar>
              <v-avatar class="mr-5 ">
                <img src="/pinterest.png">
              </v-avatar>
            </router-link>
              <span > <p class="mt-5 caption white--text">&copy; 2023 Freeeze. All Rights Reserved.</p> </span>
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


<style lang="stylus" scoped>
.backCol {
  background-color: #eae7e8;
}
</style>

<style lang="stylus" scoped>
.blockDis {
  text-align: center;
}
</style>

<style lang="stylus" scoped>
.blockIcons {
  margin-right: 160px;
}
</style>

<style lang="stylus" scoped>
.imageSth {
  margin-top: -160px;
	float: right; 
}
</style>

<style lang="stylus" scoped>
.maxWid {
  max-width: 800px; 
}
</style>

<style lang="stylus" scoped>
.iconText00 {
  font-family: "Lato", Sans, serif;
  font-size: 20px;
  font-weight: normal;
  margin-right: 770px;
}
</style>

<style lang="stylus" scoped>
.iconText11 {
  font-family: "Lato", Sans, serif;
  font-size: 20px;
  font-weight: normal;
  margin-top: -28px;
  margin-right: 690px;
  float: right;
}
</style>

<style lang="stylus" scoped>
.iconText22 {
  font-family: "Lato", Sans, serif;
  font-size: 20px;
  font-weight: normal;
  margin-top: -30px;
  margin-right: 495px;  
  float: right;
}
</style>

<style lang="stylus" scoped>
.iconText33 {
  font-family: "Lato", Sans, serif;
  font-size: 20px;
  font-weight: normal;
  margin-top: -30px;
  margin-right: 260px;
  float: right;
}
</style>


<style lang="stylus" scoped>
.footerWid {
  margin-top: 70px;
}
</style>

<style lang="stylus" scoped>
.fontTool {
  font-family: "Lato", Sans, serif;
  font-size: 15px;
  font-weight: normal;
  color:  #7a6666;;
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

