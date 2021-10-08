<template>
  <div class="test">
    <v-carousel height="828" hide-delimiter-background show-arrows-on-hover>
      <v-carousel-item
        v-for="(slide, i) in slides"
        :key="i"
        style="height: 100%"
      >
        <div class="test">
          <!-- <v-sheet v-if="i != 0" :color="colors[i]" height="100%">
            <v-row class="fill-height" align="center" justify="center">
              <div class="text-h2">{{ slide }}</div>
            </v-row>
          </v-sheet> -->
          <v-sheet v-if="i == 0" height="100%">
            <v-img :src="items[i].src" class="test">
              <v-row class="fill-height" align="center" justify="center">
                <div class="text-h2" style="margin-bottom: 390px">
                  <span class="font-test">{{ slide }}</span>
                </div>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 1" height="100%">
            <v-img :src="items[i].src" class="test">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 350px">
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">have</span>
                  </div>
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">something</span>
                  </div>
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">to tell you</span>
                  </div>
                </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 2" height="100%">
            <v-img :src="items[i].src" class="test">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px">
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">you are so</span>
                  </div>
                  <!-- <div class="text-h2" align="center" justify="center">
                    <span class="font-test">are so</span>
                  </div> -->
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">ADORABLE!!</span>
                  </div>
                </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 3" height="100%">
            <v-img :src="require('~/assets/1.jpg')">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px"> </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 4" height="100%">
            <v-img :src="require('~/assets/2.jpg')">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px"> </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 5" height="100%">
            <v-img :src="require('~/assets/3.jpg')">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px"> </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 6" height="100%">
            <v-img
              src="https://static.statusqueen.com/mobilewallpaper/thumbnail/mobile_wallpaper47-600.jpg"
              class="test"
            >
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 260px">
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">thank you for</span>
                  </div>
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">always being</span>
                  </div>
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">there for me</span>
                  </div>
                </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 7" height="100%">
            <v-img :src="require('~/assets/4.jpg')">
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px"> </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 8" height="100%">
            <v-img
              src="https://i.pinimg.com/1200x/8a/4d/3e/8a4d3e98e9462f696586396f92049a20.jpg"
              class="test"
            >
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px">
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">Finally</span>
                  </div>
                </v-col>
              </v-row>
            </v-img>
          </v-sheet>
          <v-sheet v-else-if="i == 9" height="100%">
            <v-img
              src="https://bestwallpapers.net/wp-content/uploads/2020/02/Cute-Wallpapers-Free-Download-for-Phone.jpg"
              class="test"
            >
              <v-row class="fill-height" align="center" justify="center">
                <v-col style="margin-bottom: 390px">
                  <div class="text-h2" align="center" justify="center">
                    <span class="font-test">I LOVE YOU</span>
                  </div>
                </v-col>
              </v-row>
            </v-img>
          </v-sheet>
        </div>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<style scoped>
.test {
  height: 828px !important;
}

.font-test {
  font-family: "Roboto";
  /* font-weight: bold; */
}
</style>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://i.pinimg.com/736x/f5/de/c4/f5dec4e4e02484a0628a1b518a0e4122.jpg",
        },
        {
          src: "https://i.pinimg.com/564x/16/64/dc/1664dcf929338329fd32faf40aa4ff4c.jpg",
        },
        {
          src: "https://i.pinimg.com/736x/58/75/88/587588e93670760b07ad4119485153da.jpg",
        },
        {
          src: `@/assets/1.jpg`,
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
        {
          src: `@/assets/1.jpg`,
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
        {
          src: `@/assets/1.jpg`,
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
      slides: [
        "Hi Jenny",
        "have something to tell you",
        "Third",
        "Fourth",
        "Fifth",
        "Six",
        "Seven",
        "Eight",
        "Nine",
        "Ten",
      ],
    };
  },
};
</script>