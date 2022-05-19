<template>
  <div mt-1>
        <v-subheader class="black--text text-h6">
        New Releases
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
    name:"CardCarousel1",
    data(){
        return {
            images: [
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/Bp1bAynb02/1bAyA9A4b0/size_m.jpg",
            caption:"Atm Machine"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/oAJbDElKnL/JbDEzQDjKn/size_m.jpg",
            caption:"Parada Daari"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/YoEWlwa3zX/EWlwnZRn3z/size_m.jpg",
            caption:"Honest"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/Rz4W87v3xD/4W8eO0R9bx/size_m.jpg",
            caption:"The Hook Up"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/qaLKY23pO4/LKY6nj0p3p/size_m.jpg",
            caption:"Dhoom 10"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/ogNWkDbmXJ/NWkLvEl8bm/size_m.jpg",
            caption:"Mika Singh"
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