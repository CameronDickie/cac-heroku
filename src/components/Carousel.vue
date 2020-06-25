<template>
  <v-carousel
  cycle
  height="100vh"
  interval="8000"
  hide-delimiter-background
  show-arrows-on-hover
  >
    <!-- <v-carousel-item
    v-for="(slide, i) in slides"
    :key="i"
    
    >
      <v-sheet
      :color="colors[i]"
      height="100%">
      <v-row
        class="fill-height"
        align="center"
        justify="center"
        >
        <div class="display-3">{{ slide }} Slide</div>
          <v-img contain :src="imgs[i]"></v-img>
        </v-row>
      </v-sheet>
    </v-carousel-item> -->
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    >
    </v-carousel-item>
  </v-carousel>
</template>

<script>

// var hooder = require('../assets/hooder.png');
var imgs = [
  require("../assets/media-content/imgs/img-1.jpg"),
  require("../assets/media-content/imgs/img-3.jpg"),
  require("../assets/media-content/imgs/img-4.jpg"),
  require("../assets/media-content/imgs/img-5.jpg"),
  require("../assets/media-content/imgs/img-6.jpg")
]
  export default {
    name: 'Carousel',
    data () {
      return {
        colors: [
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ],
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
        items: [
          {
            src: imgs[0],
          },
          {
            src: imgs[1],
          },
          {
            src: imgs[2],
          },
          {
            src: imgs[3],
          },
          {
            src: imgs[4]
          }
        ]
      }
    },
  }
</script>