<template>
  <v-container>
    <v-row align="center" class="row--35">
      <v-col lg="5" md="5" cols="12">
        <div class="thumbnail">
          <slot name="thum-img"></slot>
        </div>
      </v-col>
      <v-col lg="7" md="7" cols="12">
        <div class="about-inner inner">
          <div class="section-title">
            <h2 class="heading-title">About</h2>
            <p class="description">
              Hey there again, I am a designer with education background in fashion and multimedia. I am open minded and hard worker. Moving forward and always looking for new ways to any problems. Innovation is what I strive for. 
            </p>
          </div>
          <v-row class="mt--30 mt_sm--10">
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="about-us-list">
                <h3 class="heading-title">
                  Who we are
                </h3>
                <p>
                  There are many vtions of passages of Lorem Ipsum available,
                  but the majority have suffered.
                </p>
              </div>
            </v-col>
            <v-col lg="6" md="6" sm="12" cols="12">
              <div class="about-us-list">
                <h3 class="heading-title">
                  Who we are
                </h3>
                <p>
                  There are many vtions of passages of Lorem Ipsum available,
                  but the majority have suffered.
                </p>
              </div>
            </v-col>
          </v-row>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
