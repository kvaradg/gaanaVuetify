<template>
 <!-- <v-flex>
      <v-card outlined width="250px">
      <v-card-title v-for="image in images" :key="image.link">
        <v-img :src="image.link"></v-img>
      </v-card-title>
  <v-card-subtitle>Dua Lipa</v-card-subtitle>
</v-card>
 </v-flex> -->


 <!-- <v-carousel hide-delimiters>
      <v-carousel-item   v-for="image in images" :key="image.link">
        <v-sheet :color="color" height="100%" tile>
          <v-row class="fill-height" align="center" justify="center">
            <div class="text-h2">
                <v-img class="img" :src="image.link"></v-img>
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel> -->

    <div mx-1>
        <v-subheader class="black--text text-h6">
        Trending Songs
    </v-subheader>
<v-row>
    <v-col  lg="2" v-for="image in images" :key="image.link" >
       <v-img class="rounded-img" :src="image.link"></v-img>
       <p>{{image.caption}}</p>
    </v-col>
</v-row>
    </div>
</template>

    <script>
    export default {
    name:"CardCarousel",
    data(){
        return {
            images: [
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/kGxbnw0Ky4/xbnw6AmoKy/size_m.jpg",
            caption:"The Last Ride"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/song/d41WjnWPLq/1WjBydDAWP/size_m_1651113191.webp",
            caption:"The Drum"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/Rz4W87v3xD/4W8edjAObx/size_m.jpg",
            caption:"Cooped Up"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/6Zxb2r7b9w/xb2rZ4kwb9/size_m_1651117834.webp",
            caption:"De Taali"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/9MAWe7KyJe/AWe9Jw5wWy/size_m.jpg",
            caption:"Bhool Bhulliya 2"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/Rz4W87v3xD/4W8eOzGvbx/size_m.jpg",
            caption:"Love Me Back"
            },
        ],
        }
    }
    }
    </script>

    <style>
    .rounded-img{
        border-radius: 10px;
        margin:10px;
    }
    </style>