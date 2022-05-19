<template>
<div d-flex justify-center>
   <hr>
   <!-- <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="white black--text text-center"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 black--text"
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="black--text pt-0">
        Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="black--text">
        {{ new Date().getFullYear() }} — <strong>Gaana.com</strong>
      </v-card-text>
    </v-card>
  </v-footer> -->
   <v-footer
      color="black"
      dark
    >
      <v-row
        justify="center"
        class="my-4 text-center"
      >

    <v-col cols="12 text-h6"
          >Bas Bajna Chahiye Gaana</v-col
        >
      
        <v-col cols="12"
          >Gaana is the one-stop solution for all your music needs. Gaana offers you free, unlimited access to over 30<br> 
          million Hindi Songs, Bollywood Music, English MP3 songs, Regional Music & Mirchi Play.</v-col
        >
        <v-col cols="12">
          <v-btn
            v-for="icon in icons"
            :key="icon"
            text
            dark
          >
            <v-icon>{{ icon }}</v-icon>
          </v-btn>
        </v-col>
        <v-col
          cols="12"
          class="align-center"
          >&copy; 2022 Gaana.com</v-col
        >
      </v-row>
    </v-footer>
</div>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>

<style>
.title{
    text-align: center;
}
</style>