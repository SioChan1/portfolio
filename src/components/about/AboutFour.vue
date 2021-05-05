<template>
  <v-row class="row--35" align="center">
    <v-col lg="5" md="5" cols="12">
      <div class="thumbnail">
        <slot name="thum-img"></slot>
      </div>
    </v-col>
    <v-col lg="7" md="7" cols="12">
      <div class="about-inner inner pt--100 pt_sm--40 pt_md--40">
        <div class="section-title">
          <h2 class="heading-title">About Me</h2>
          <p class="description">
            Hey there again, I am a designer with an education background in fashion and multimedia design. I am open minded and hard worker, that gets along well with others. Moving forward and always looking for new ways to solve problems. Innovation is what I strive for. 
I am not shy to take a lead in projects, but as well I am great at following lead of others.
          </p> 
<div> 
  <section> 
    <iframe width="560" height="315" src="https://www.youtube.com/embed/xiME2jThR18" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </section>
</div>
 

        </div>
        <!-- End .section-title -->
        <div class="tab-wrapper mt--30">
          <v-row>
            <TabTwo />
          </v-row>
        </div>
      </div>
    </v-col>
  </v-row>
</template>

<script>
  import TabTwo from "../../components/tabs/TabTwo";
  export default {
    components: { TabTwo },
    data() {
      return {};
    },
  };
</script>
