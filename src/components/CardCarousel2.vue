<template>
  <div mt-1>
        <v-subheader class="black--text text-h6">
            Top Charts
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
    name:"CardCarousel2",
    data(){
        return {
            images: [
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/01A3mrWNQX/A3mO66mzbN/size_m_1649757782.webp",
            caption:"EDM Top-50"
            },
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/jBr3gybR1m/r3gmPRNybR/size_m_1641546010.webp",
            caption:"Bhakti Top-50"
            },
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/zLp36v3rGe/Lp36kP5NWr/size_m_1650280045.webp",
            caption:"Romance Top-50"
            },
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/oAJbDElKnL/JbDEDR0lKn/size_m_1650626439.webp",
            caption:"International Top-50"
            },
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/w4MKPgOboj/4MKP2xArWo/size_m_1652774274.webp",
            caption:"Punjabi Top-50"
            },
            {
            link: "https://a10.gaanacdn.com/gn_pl_img/playlists/P7m3GNKqxo/7m3GQwOybq/size_m_1652775743.webp",
            caption:"Hindi Top-50"
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