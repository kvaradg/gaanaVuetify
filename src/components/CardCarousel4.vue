<template>
  <div>
        <v-subheader class="black--text text-h6">
            Featured Artists
    </v-subheader>
<v-row>
    <v-col  lg="2"  v-for="image in images" :key="image.link" >
       <v-img class="rounded-img" :src="image.link"></v-img>
       <p class="text-center">{{image.caption}}</p>
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
            link: "https://a10.gaanacdn.com/gn_img/artists/Rz4W87v3xD/Rz4W8ppWxD/size_m_1638817418.webp",
            caption:"Neha Kakkar"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/artists/10q3ZR1352/0q3Z6Lg135/size_m_1638777310.webp",
            caption:"Jubin Nautiyal"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/artists/w4MKPDOKoj/4MKPgoQgbo/size_m_1516802409.webp",
            caption:"Honey Singh"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/artists/zLp36PvbrG/Lp36AR0KrG/size_m_1516707336.webp",
            caption:"Pritam"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/artists/21GWwrR3pk/1GWwYz4DKp/size_m_1567610470.webp",
            caption:"Tanishq Baci"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/artists/Dk9KNk23Bx/k9KNqJJbBx/size_m_1638898900.webp",
            caption:"Arijit Singh"
            },
        ],
        }
    }
    }
    </script>

    <style scoped>
    .rounded-img{
        border-radius: 100%;
        margin:10px;
    }
    
    </style>