<template>
  <div class="about">
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
          <router-link to="/">
            <span class="mr-5 fontTool">Home</span>
          </router-link>
          <span class="mr-5 fontTool">About</span>
          <span class="mr-5 fontTool">Blog</span>
          <span class="mr-2 fontTool">Contact</span>  
        </v-toolbar-title>
      </v-layout>
    </v-toolbar>
    <div>
      <v-layout row wrap class="blockDis widContact">
        <v-flex class="lime darken-1" > 
          <v-container  class="white--text ">
            <h1 class="iconText00"> CONTACT</h1>
          </v-container>
        </v-flex>
      </v-layout>
    </div>
    <div>
      <img src="/map.jpg" alt="">
      <img src="/bg-transparent.png" class="imageTrans" alt="">
      <div class="imageMap">
        <img src="/check-in.png" alt="">
        <h1 class="fontBod pink--text">UNIT 0123 , ABC BUILDING, BUSSINESS PARK</h1>
        <p class="body-1">If you're having problems editing this website template, then don't hesitate to ask for help on the Forums.</p>
      </div>
    </div>
    <div class="marginPage">
      <h1 class="mt-5 ml-3 fontBod pink--text">INQUIRY FORM</h1>
      <v-form>
        <v-container>
          <v-flex xs12 sm6>
            <v-text-field
              v-model="message2"
              solo
              label="Name"
              clearable
            ></v-text-field>
          </v-flex>
          <v-flex xs12 sm6>
            <v-text-field
              v-model="message2"
              solo
              label="Email"
              clearable
            ></v-text-field>
          </v-flex>
          <v-flex xs12 sm6  >
            <v-text-field
              v-model="message2"
              solo
              label="Subject"
              clearable
            ></v-text-field>
          </v-flex> 
          <v-flex xs12 sm6  >
            <v-text-field
              v-model="message2"
              solo
              label="Share your thoughts"
              multi-line
              clearable
            ></v-text-field>
          </v-flex>
          <v-btn outline color="green ">SEND</v-btn>
        </v-container>
      </v-form>
      <div class="section">
        <h1 class="fontBod pink--text blockDis mt-2">WE’D LOVE TO HEAR FROM YOU.</h1>
        <p  class="body-1 blockDis ml-2 mr-2 mt-2">If you're having problems editing this website template, then don't hesitate to ask for help on the Forums.</p>
      </div>
    </div>
    <v-footer  >
      <v-layout row wrap class="blockDis footerWid">
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

<style lang="stylus" scoped>
.fontTool {
  font-family: "Lato", Sans, serif;
  font-size: 15px;
  font-weight: normal;
  color:  #7a6666;;
}
</style>

<style lang="stylus" scoped>
.fontBod {
  font-family: "Lato", Sans, serif;
  font-size: 24px;
  font-weight: normal;
  color:  #7a6666;;
}
</style>

<style lang="stylus" scoped>
.iconText00 {
  font-family: "Lato", Sans, serif;
  font-size: 30px;
  font-weight: normal;
}
</style>

<style lang="stylus" scoped>
.widContact {
  width: 100%;
  height: 90px;
}
</style>

<style lang="stylus" scoped>
.footerWid {
  margin-top: 250px;
}
</style>


<style lang="stylus" scoped>
.imageMap {
  margin-top: -260px;
  margin-left: 450px;
	max-width: 960px;
	overflow: hidden;
	padding: 39px 0 0;
}
</style>

<style lang="stylus" scoped>
.imageTrans {
  margin-top: -300px;
  margin-left: 250px; 
  overflow: hidden;
  padding: 30px 0 35px 133px;
  height: 250px;
  width: 890px;
}
</style>

<style lang="stylus" scoped>
.marginPage {
  margin-left: 365px; 
}
</style>

<style lang="stylus" scoped>
.section {
  background-color: #EFEDEE;
	margin-top: -480px;
  margin-left: 600px;
	max-width: none;
	padding: 0 0 35px;
	width: 280px;
	float: left;
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