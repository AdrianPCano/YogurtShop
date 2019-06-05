<template>
  <div class="about">
    <v-toolbar class="grey lighten-2" flat height = "120">
      <v-layout justify-space-around>
        <router-link to="/">
          <v-image v-for="image in image" :key="image.image">
            <img :src="image.logo">
          </v-image>
        </router-link>
      </v-layout>
      <v-layout justify-space-around>
        <v-toolbar-title class="headline text-uppercase">
          <router-link to="/">
            <span class="mr-5">Home</span>
          </router-link>
          <span class="mr-5">About</span>
          <span class="mr-5">Blog</span>
          <span class="mr-2">Contact</span>  
        </v-toolbar-title>
      </v-layout>
    </v-toolbar>
    <v-container class="my-5">
    </v-container>
    <v-footer  class="blockDis" >
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
.imageSth {
  margin-top: -150px;
	float: right; 
}
</style>

<style lang="stylus" scoped>
.maxWid {
  max-width: 800px; 
}
</style>



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