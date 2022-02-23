<template>
  <div class="">
    <v-carousel cycle height="100%" :show-arrows="false">
      <v-sheet height="100%">
      <v-carousel-item v-for="(item, i) in items" :key="i">
        <v-img height="100%" class="shrink" :src="item.src">
          <!-- <v-row align="center" justify="center" class="pa-8" style="height: 80vh;">
      <v-col cols="12" md="4" lg="6" sm="12" class="banner-text">
        <div align="center">
        <div class="ma-lg-4 text-h3">
         {{ item.text }}
        </div>
        <div>
          <v-btn width="150" rounded>
            Enroll
          </v-btn>
        </div>
        </div>
      </v-col>
    </v-row> -->
        </v-img>
      </v-carousel-item>
      </v-sheet>
    </v-carousel>
    <!-- <v-container fluid>
    </v-container> -->
  </div>
</template>

<script>
// import VueHtmlEditor from 'vue-html-editor'
export default {
  name: 'HomePage',
  components: {},
  data () {
    return {
      video: ['Zoom', 'Google Meet'],
      text: 'Hello World!',
      level: [
        'Beginner',
        'Between Beginner and Intermediate',
        'Intermediate',
        'Above Intermediate'
      ],
      preferredHours: ['Morning', 'Afternoon', 'Evening'],
      items: [
        {
          src: require('../assets/invites/anniversary-banners.jpg'),
          text: 'Skill-up with our Javascript Developer sessions. '
        },
        {
          src: require('../assets/invites/anniversary-banners-2.jpg'),
          text: 'Practical sessions to speed your expertise on how things work'
        },
        {
          src: require('../assets/invites/anniversary-banners-3.jpg'),
          text:
            'Experience real-world agile software development with your team'
        }
      ]
    }
  }
}
</script>

<style scoped>
.option {

  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
}
.banner-text {
}
</style>
