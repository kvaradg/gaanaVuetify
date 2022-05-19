<template>
  <v-app>
    <v-app-bar flat app>
      <v-app-bar-nav-icon @click="isToggle = !isToggle"></v-app-bar-nav-icon>
      <v-icon></v-icon>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-spacer></v-spacer>

      <span class="body-2 mr-4 pa-2 red--text">Go Add Free</span>
      <span class="body-2 mr-4 pa-2 red--text">Get Gaana Plus</span>
      <v-icon class="mr-2">translate</v-icon>
      <v-icon class="mr-2">dark_mode</v-icon>
      <span class="body-2">Log In/Sign Up</span>
    </v-app-bar>

    <!-- Carousel  -->
    <!-- <v-carousel hide-delimiters>
      <v-carousel-item   v-for="image in images" :key="image.link">
        <v-sheet :color="color" height="100%" tile>
          <v-row class="fill-height" align="center" justify="center">
           
                 <div class="text-h2 carousel-img">
                <v-img class="img" :src="image.link"></v-img>
                 <v-img class="img" :src="image.link"></v-img>
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel> -->

    <MainCarousel1/>

    <CardCarousel/>
    <CardCarousel1/>
    <CardCarousel2/>
    <CardCarousel3/>
    <CardCarousel4/>
    <CardCarousel5/>
    <FoooterComp/>
    <!-- -------------------navigation drawer-------------------- -->
    <v-navigation-drawer app v-model="isToggle">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h7">
            <v-icon class="item-padding" size="45">account_circle</v-icon>
            <span class="item-padding">Login/Signup</span>
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-content>
            <span class="item-padding">Home</span>
            <span class="item-padding">Radio</span>
            <span class="item-padding">Podcast</span>
            <span class="item-padding">My Music</span>
            <span class="item-padding">India's Music</span>

            <v-list-item-title>
              <span class="item-padding">Language</span>
            </v-list-item-title>
            <v-list-item-subtitle>(Set Music Language)</v-list-item-subtitle>
            <v-list-item-title class="item-padding">
              <span class="item-padding">Night Mode</span>
              <v-icon size="60">toggle_off</v-icon>
            </v-list-item-title>
            <v-divider class="item-padding"></v-divider>
            <v-list-item-title class="text-h6">
              <span class="item-padding">Go Premium</span>
            </v-list-item-title>
            <span class="item-padding">Go Ad-Free</span>
            <span class="item-padding"> Get Gaana Plus</span>
            <v-divider class="item-padding"></v-divider>

            <v-list-item-title class="text-h6">
              <span class="item-padding">Quick Access</span>
            </v-list-item-title>
            <span class="item-padding">Trending Songs</span>
            <span class="item-padding">New Songs</span>
            <span class="item-padding">Old Songs</span>
            <span class="item-padding">Album</span>
            <span class="item-padding"> Artist</span>
            <span class="item-padding">Lyrics</span>
            <span class="item-padding">Music Labels</span>
            <span class="item-padding">Genres</span>

            <v-divider></v-divider>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <router-view></router-view>
  </v-app>
</template>

<script>
import CardCarousel from './CardCarousel.vue';
import CardCarousel1 from './CardCarousel1.vue';
import CardCarousel2 from './CardCarousel2.vue';
import CardCarousel3 from './CardCarousel3.vue';
import CardCarousel4 from './CardCarousel4.vue';
import CardCarousel5 from './CardCarousel5.vue';
import FoooterComp from './FoooterComp.vue';
import MainCarousel1 from './MainCarousel1.vue';
export default {
    name: "NavBar",
    data() {
        return {
            isToggle: false,
            // images: [
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/81l3Mye3rM/1l3M746brM/size_s_1634647664.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/D0PKLrWGl9/0PKLokqbGl/size_s_1603722608.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/ZaP374RWDy/ZaP372BKDy/size_s_1641541612.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/ogNWkDbmXJ/gNWklzJbmX/size_s_1649439625.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/81l3Mye3rM/1l3M746brM/size_s_1634647664.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/VdNW0JMKo5/dNW0ljwWo5/size_s_1649440070.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/DwPKOxB3qV/wPKOze6bqV/size_s_1593003531.webp",
            //     },
            //     {
            //         link: "https://a10.gaanacdn.com/gn_img/showcase/MmqK5EKwRO/mqK5MY1KwR/size_s_1631642131.webp",
            //     },
            // ],
            
        };
    },
    methods: {
        toggle() {
            this.isToggle = "true";
        },
    },
    
    components: { CardCarousel, CardCarousel1, CardCarousel2, CardCarousel3, CardCarousel4, CardCarousel5, FoooterComp, MainCarousel1 }
};
</script>

<style>
.item-padding {
  padding: 15px;
}
.img{
    height: 300px;
    width: 700px;
}
.carousel-img{
    display: flex;
}
</style>
