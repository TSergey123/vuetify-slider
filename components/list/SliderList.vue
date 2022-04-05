<template>
    <v-sheet
      class="mx-auto"
      elevation="0"
      style="background-color: transparent;"
    >
      <v-slide-group
        class="ml-0"
        center-active
        show-arrows
        dark
      >
          <v-row justify="center" align="center" class="my-1">
            <v-slide-item
              v-slot="{ toggle }"
              v-for="(card, index) in cards"
              :key="index"
              class="ml-1 mr-1 slide-item-card"
            >
              <div
                class="slider-item"
                v-on:click="toggleCard(card)"
                @click="toggle"
              >
                <div>
                  <transition name="flip">
                    <div v-bind:key="card.flipped" class="card">
                      <img
                        v-if="!card.flipped"
                        width="100"
                        height="100"
                        :src="card.toolLogo"
                        alt="logo"
                      />
                      <p>
                        {{
                          card.flipped ? card.companyName : card.positionTitle
                        }}
                      </p>
                      <a
                        v-if="card.flipped"
                        :href="card.projectLink"
                        >{{card.cardLink}}</a
                      >
                      <p>{{ card.flipped ? null : card.jobDate }}</p>
                    </div>
                  </transition>
                </div>
              </div>
            </v-slide-item>
          </v-row>
      </v-slide-group>
    </v-sheet>
</template>

<script>
export default {
  name: 'SliderList',
  props: {
    cards: {
      type: Array,
    },
  },
  methods: {
    toggleCard: function (card) {
      card.flipped = !card.flipped
    },
  },
}
</script>
<style>
ul {
  padding-left: 0;
  display: flex;
  flex-flow: row wrap;
}

.slide-item {
  list-style-type: none;
  padding: 10px 10px;
  transition: all 10s ease;
}

.container {
  max-width: 100%;
  padding: 2em;
}

.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  width: 15rem;
  height: 15rem;
  background-color: #51aae5;
  border-radius: 7px;
  margin: 5px;
  cursor: pointer;
  position: relative;
  color: #fff;
  font-weight: 600;
  font-size: 20px;
  will-change: transform;
}

.slider-item:hover {
  transform: scale(1.1);
  z-index: 999;
  outline: 1px solid black;
}

.slider-item:nth-child(-n + 3) .card {
  background-color: #e65f51;
}

.slider-item:nth-child(2n + 1) .card {
  background-color: #a17de9;
}

.slider-item:nth-child(4n) .card {
  background-color: #feca34;
}

.slider-item:nth-child(5n-2) .card {
  background-color: #51aae5;
}

.slider-item:nth-child(4n + 4) .card {
  background-color: #feca34;
}

.slider-item:nth-child(-7n + 7) .card {
  background-color: #e46055;
}

.flip-enter-active {
  transition: all 1s ease;
}

.flip-leave-active {
  display: none;
}

.flip-enter,
.flip-leave {
  transform: rotateY(360deg);
  opacity: 1;
}

/* Form */
.flashcard-form {
  position: relative;
}

label {
  font-weight: 400;
  color: #333;
  margin-right: 10px;
}

input {
  border-radius: 5px;
  border: 2px solid #eaeaea;
  padding: 10px;
  outline: none;
}

button {
  border-radius: 5px;
  border: 1px solid #87cb84;
  background-color: #87cb84;
  padding: 8px 15px;
  outline: none;
  font-size: 14px;
  font-weight: 700;
  color: #fff;
  cursor: pointer;
  transition: all 10s ease;
}

button:hover {
  background-color: #70a66f;
}

.error {
  margin-top: 10px;
  display: block;
  color: #e44e42;
  font-weight: 600;
}
</style>
