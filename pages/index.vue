<template>
  <v-app>
    <v-container style="height: 100%">
      <v-row align="center" style="height: 100%">
        <v-col cols="12" class="pl-0 pr-0" align="center">
          <h1 class="text">Work Experince</h1>
          <ListSliderList :cards="positions" />
          <h1 class="mt-5">Pet Projects</h1>
          <ListSliderList :cards="projects" />
          <ContactInfoList />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      positions: [
        {
          companyLogo: 'v.png',
          toolLogo: 'v.png',
          positionTitle: 'Vue developer',
          jobDate: '2022-2022',
          companyName: 'Rshb-intech',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'qa.png',
          toolLogo: 'qa.png',
          positionTitle: 'Senior QA Engineer',
          jobDate: '2018-2022',
          companyName: 'TechnoProgress',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'v.png',
          toolLogo: 'qa.png',
          positionTitle: 'Middle QA Engineer',
          jobDate: '2017-2018',
          companyName: 'SberTech',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'v.png',
          toolLogo: 'qa.png',
          positionTitle: 'Junior QA Engineer',
          jobDate: '2016-2017',
          companyName: 'MTC-communications',
          companyLink: 'https://google.com',
          flipped: false,
        },
      ],
      projects: [
        {
          toolLogo: 'v.png',
          positionTitle: 'E-Shop',
          projectLink: 'https://gilded-bienenstitch-3fac67.netlify.app/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'react.png',
          positionTitle: 'Google Books',
          projectLink: 'https://tsergey123.github.io/my-new-app/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'v.png',
          positionTitle: 'Post List',
          projectLink: 'https://tsergey123.github.io/vue-playground/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'v.png',
          positionTitle: 'Online Shop',
          projectLink: 'https://tsergey123.github.io/vue-popup/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'react.png',
          positionTitle: 'What to watch',
          projectLink: 'https://tsergey123.github.io/what-to-watch/index.html',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'react.png',
          positionTitle: 'React Native To Do',
          projectLink:
            'https://tsergey123.github.io/react-native-todolist-portfolio/index.html',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'js.svg',
          positionTitle: 'Cinemaddict',
          projectLink: 'https://tsergey123.github.io/cinemaddict/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'js.svg',
          positionTitle: 'Booking',
          projectLink:
            'https://tsergey123.github.io/Keksobooking/build/index.html',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'js.svg',
          positionTitle: 'Calorie Counter',
          projectLink: 'https://tsergey123.github.io/calorie-counter/',
          flipped: false,
          cardLink: 'Project Link'
        },
        {
          toolLogo: 'js.svg',
          positionTitle: 'Endless Carousel',
          projectLink: 'https://tsergey123.github.io/infinity-carousel/',
          flipped: false,
          cardLink: 'Project Link'
        },
      ],
    }
  },
}
</script>
<style>
#app {
  background-color: #1a1b21;
}
h1 {
  color: #fff;
}
</style>
