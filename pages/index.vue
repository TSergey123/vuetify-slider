<template>
  <v-app>
    <v-sheet class="mx-auto" width="50%" elevation="7">
      <v-slide-group v-model="model" class="pa-4">
        <v-slide-item>
          <v-card
            :color="active ? 'primary' : 'grey lighten-1'"
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide1</h1>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item>
          <v-card
            :color="active ? 'primary' : 'grey lighten-1'"
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide2</h1>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item>
          <v-card
            :color="active ? 'primary' : 'grey lighten-1'"
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide3</h1>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item>
          <v-card
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide4</h1>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item>
          <v-card
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide</h1>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item>
          <v-card
            :color="active ? 'primary' : 'grey lighten-1'"
            class="ma-4"
            height="300"
            width="300"
          >
            <v-row class="fill-height" align="center" justify="center">
              <h1>slide</h1>
            </v-row>
          </v-card>
        </v-slide-item>
      </v-slide-group>
    </v-sheet>
  </v-app>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      colors: ['red', 'blue', 'green'],
    }
  },
}
</script>
<style>
.carousel__controls {
  display: none;
}
</style>
