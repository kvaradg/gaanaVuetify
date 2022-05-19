<template>
  <v-carousel hide-delimiters> 
        <template v-for="(item, index) in slider"> 
          <v-carousel-item v-if="(index + 1) % columns === 1 || columns === 1" 
                           :key="index"
          > 
            <v-row class="flex-nowrap" style="height:100%"> 
              <template v-for="(n,i) in columns"> 
                <template v-if="(+index + i) < slider.length"> 
                  <v-col :key="i"> 
                    <v-img v-if="(+index + i) < slider.length" 
                             :src="slider[+index + i]"
                             height="100%"
                    >
                      <v-row
                             align="center"
                             justify="center"
                      >
                    
                      </v-row>
                    </v-img>
                  </v-col> 
                </template> 
              </template> 
            </v-row> 
          </v-carousel-item> 
        </template> 
      </v-carousel> 
</template>

<script>
export default {
name:"MainCarousel",
data(){
    return{
        slider: [
        "https://a10.gaanacdn.com/gn_img/showcase/81l3Mye3rM/1l3M746brM/size_s_1634647664.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/D0PKLrWGl9/0PKLokqbGl/size_s_1603722608.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/ZaP374RWDy/ZaP372BKDy/size_s_1641541612.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/ogNWkDbmXJ/gNWklzJbmX/size_s_1649439625.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/81l3Mye3rM/1l3M746brM/size_s_1634647664.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/VdNW0JMKo5/dNW0ljwWo5/size_s_1649440070.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/DwPKOxB3qV/wPKOze6bqV/size_s_1593003531.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/MmqK5EKwRO/mqK5MY1KwR/size_s_1631642131.webp", 
        "https://a10.gaanacdn.com/gn_img/showcase/D0PKLrWGl9/0PKLokqbGl/size_s_1603722608.webp", 
      ],
    }   
},
computed: {
    columns() {
      if (this.$vuetify.breakpoint.xl) {
        return 4;
      }

      if (this.$vuetify.breakpoint.lg) {
        return 3;
      }

      if (this.$vuetify.breakpoint.md) {
        return 2;
      }

      return 1;
    }
  },

}
</script>

<style>

</style>