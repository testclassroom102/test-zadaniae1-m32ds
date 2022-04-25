<template>
  <div>
    <!--AppBar duży-->
    <v-app-bar class="hidden-sm-and-down" fixed flat color="transparent">
      <v-layout justify-center>
       
       
       <v-card  style="cursor: pointer" href="/" height="40px" color="transparent" flat>
         <img src="@/assets/logo1.png"  height="40px">
       </v-card>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#o-nas')" rounded text dark>O NAS</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#certyfikaty')" rounded text dark>CERTYFIKATY</v-btn>
   
    
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#oferta')" rounded text dark>OFERTA</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#gdzie-kupic')" rounded text dark>GDZIE KUPIĆ</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#kontakt')" rounded text dark>KONTAKT</v-btn>
      </v-layout>
    </v-app-bar>

       <v-app-bar class="hidden-sm-and-down" fixed inverted-scroll flat color="white">
      <v-layout justify-center>
         <v-card style="cursor: pointer" href="/" height="40px" color="transparent" flat>
         <img src="@/assets/logo1.png"  height="40px">
       </v-card>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#o-nas')" rounded text color="#0D47A1" dark>O NAS</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#certyfikaty')" rounded text color="#0D47A1" dark>CERTYFIKATY</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#oferta')" rounded text color="#0D47A1" dark>OFERTA</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#gdzie-kupic')" rounded text color="#0D47A1" dark>GDZIE KUPIĆ</v-btn>
        <v-btn class="ml-3 mt-1" @click="$vuetify.goTo('#kontakt')" rounded text color="#0D47A1" dark>KONTAKT</v-btn>
      </v-layout>
    </v-app-bar>

    <!--AppBar mały-->
    <v-app-bar class="hidden-md-and-up" fixed flat color="transparent">
      <v-layout justify-left>
        <v-btn class=" mt-1 mr-3" @click="drawer = !drawer" style="border-radius: 8px" color="blue darken-4" dark
          ><v-icon>mdi-menu</v-icon></v-btn>
               <v-card style="cursor: pointer" href="/" height="40px" color="transparent" flat>
         <img src="@/assets/logo1.png"  height="40px">
       </v-card>
      </v-layout>
    </v-app-bar>

      <v-app-bar class="hidden-md-and-up" fixed flat color="white" inverted-scroll>
      <v-layout justify-left>
        <v-btn class=" mt-1 mr-3" @click="drawer = !drawer" style="border-radius: 8px" color="#0D47A1" dark
          ><v-icon>mdi-menu</v-icon></v-btn>
              <v-card style="cursor: pointer" href="/" height="40px" color="transparent" flat>
         <img src="@/assets/logo1.png"  height="40px">
       </v-card>
      </v-layout>
    </v-app-bar>

    <!--Navigation drawer-->
    <v-navigation-drawer fixed v-model="drawer">

      <v-layout column align-center>
       <v-card class="mt-4" style="cursor: pointer; border-radius: 10px" href="/" height="45px" color="transparent" flat>
         <img src="@/assets/logo1.png"  height="45px">
       </v-card>
      </v-layout>

      
     <v-layout class="mt-5" column justify-start>
       <v-btn class="mt-1" @click="$vuetify.goTo('#o-nas')"  text color="#0D47A1" dark>O NAS</v-btn>
        <v-btn class="mt-1" @click="$vuetify.goTo('#certyfikaty')"  text color="#0D47A1" dark>CERTYFIKATY</v-btn>
        <v-btn class="mt-1" @click="$vuetify.goTo('#oferta')"  text color="#0D47A1" dark>OFERTA</v-btn>
        <v-btn class="mt-1" @click="$vuetify.goTo('#gdzie-kupic')"  text color="#0D47A1" dark>GDZIE KUPIĆ</v-btn>
        <v-btn class="mt-1" @click="$vuetify.goTo('#kontakt')"  text color="#0D47A1" dark>KONTAKT</v-btn>
     </v-layout>
    </v-navigation-drawer>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        drawer: false,
        // items: [
        //   { title: 'O NAS', icon: 'mdi-view-dashboard', to: 'o-nas'},
        //   { title: 'CERTYFIKATY', icon: 'mdi-image', to: 'certyfikaty' },
        //   { title: 'OFERTA', icon: 'mdi-help-box', to: 'oferta' },
        //   { title: 'GDZIE KUPIĆ', icon: 'mdi-help-box', to: 'gdzie-kupic' },
        //   { title: 'KONTAKT', icon: 'mdi-help-box', to: 'kontakt' },
        // ],
        right: null,
      }
    },
  }
</script>

<style>
</style>