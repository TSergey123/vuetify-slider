<template>
  <v-app>
    <v-container style="height:100%;">
      <v-row align="center" style="height: 100%;">
        <v-col class="pl-0 pr-0" align="center">
          <h1 class="text">Work Experince</h1>
          <ListSliderList :cards="positions" />
          <h1 class="mt-5">Pet Projects</h1>
          <ListSliderList :cards="projects" />
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
          jobDate: '2020-2022',
          companyName: 'Rshb-intech',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'qa.png',
          toolLogo: 'qa.png',
          positionTitle: 'QA Engineer',
          jobDate: '2018-2020',
          companyName: 'TechnoProgress',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'v.png',
          toolLogo: 'qa.png',
          positionTitle: 'QA Engineer',
          jobDate: '2017-2018',
          companyName: 'SberTech',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          companyLogo: 'v.png',
          toolLogo: 'qa.png',
          positionTitle: 'QA Engineer',
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
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          toolLogo: 'v.png',
          positionTitle: 'OnlineShop',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          toolLogo: 'v.png',
          positionTitle: 'Todo List',
          companyLink: 'https://google.com',
          flipped: false,
        },
        {
          toolLogo: 'v.png',
          positionTitle: 'E-Shop',
          companyLink: 'https://google.com',
          flipped: false,
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
