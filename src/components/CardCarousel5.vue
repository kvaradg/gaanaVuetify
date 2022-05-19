<template>
  <div>
        <v-subheader class="black--text text-h6">
            Radio
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
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/10q3ZR1352/10q3Zm2K52/size_m_1643619359.webp",
            caption:"Morning Mix"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/0wrb4kNWLg/0wrb4jV3Lg/size_m_1643615968.webp",
            caption:"Workout"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/2lV3dl13Rg/2lV3dGZKRg/size_m_1643700049.webp",
            caption:"90s and 2000s"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/DwPKOxB3qV/DwPKOwkKqV/size_m_1643620296.webp",
            caption:"Party"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/qa4WEqWP1p/qa4WEm8WP1/size_m_1643616033.webp",
            caption:"Love Hits"
            },
            {
            link: "https://a10.gaanacdn.com/gn_img/g_radio_circle/kGxbnw0Ky4/kGxbnxJ3y4/size_m_1643619328.webp",
            caption:"Dance"
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