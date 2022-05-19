<template>
  <div>
        <v-subheader class="black--text text-h6">
            Top Charts
    </v-subheader>
<v-row>
    <v-col  lg="2"  v-for="image in images" :key="image.link" >
       <v-img class="rounded-img" :src="image.link"></v-img>
       <p>{{image.caption}}</p>
    </v-col>
</v-row>
    </div>
</template>

    <script>
    export default {
    name:"CardCarousel3",
    data(){
        return {
            images: [
            {
            link: "https://a10.gaanacdn.com/gn_img/song/4Z9bqo3yQn/9bqNj4XyKy/size_m_1593616645.webp",
            caption:"Cute Song"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/ogNWkLDbmX/NWkLm5Vkbm/size_m.webp",
            caption:"Baarish"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/a7LWBkzbzX/7LWBVPRDWz/size_m.webp",
            caption:"Teri Akkhon Mein"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/0wrb4kNWLg/wrb476lyWL/size_m.webp",
            caption:"Taaron Ke Shehar"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/song/lJvKa56KDV/vKa91Z1RKD/size_m_1628085090.webp",
            caption:"Raatan Lambiyya"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/albums/d41WjznWPL/41Wj2qgNWP/size_m.webp",
            caption:"Naach Meri Rani"
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