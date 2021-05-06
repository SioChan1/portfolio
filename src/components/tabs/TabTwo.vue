<template>
  <v-col lg="12">
    <div class="tab-default">
      <v-tabs v-model="tab" flat hide-slider>
        <v-tab v-for="item in items" :key="item.id" :ripple="false">
          {{ item.name }}
        </v-tab>
      </v-tabs>

      <v-tabs-items v-model="tab">
        <v-tab-item
          transition="fade-transition"
          v-for="item in tabContent"
          :key="item.id"
        >
          <v-card flat>
            <v-card-text>
              <div class="single-tab-content">
                <ul>
                  <li v-for="(item, i) in item.content" :key="i">
                    <router-link to=""
                      >{{ item.title }}
                      <span> - {{ item.name }}</span></router-link
                    >
                    {{ item.desc }}
                  </li>
                </ul>
              </div>
            </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs-items>
    </div>
  </v-col>
</template>
<script>
  export default {
    data() {
      return {
        tab: null,
        items: [
          {
            id: 1,
            name: "Skills",
          },
          {
            id: 2,
            name: "Personal traits",
          },
          {
            id: 3,
            name: "Experience",
          },
          {
            id: 4,
            name: "Education & Certification",
          },
        ],

        tabContent: [
          {
            id: 1,
            content: [
              {
                title: "Creative suit",
                name: "Adobe",
                desc: "Advanced understanding of the programs.",
              },
              {
                title: "Forecasting",
                name: "Trend analysis",
                desc: "Fashion studies background and internship experience in trendforecasting, using pantone method.",
              },
              {
                title: "Project management",
                name: "Teamwork",
                desc: "Experience in project management.",
              },
            ],
          },
          {
            id: 2,
            content: [
              {
                title: "Stuborn",
                name: "Will not stop until a solution to a problem is found.",
                
              },
              {
                title: "Extrovert",
                name: "No problems when it comes to talking to new people and public speaking.",
                
              },
              {
                title: "Honest",
                name: "Will always stay honest to people around me.",
                
              },
              {
                title: "Empath",
                name: "Will always find a way to listen and understand, both in a professional and personal enviroment.",
                
              },
              {
                title: "Caring",
                name: "Never find it a problem to help out others.",
                
              },
            ],
          },
          {
            id: 3,
            content: [
              {
                title: "Design Assistant",
                name: "Marc Lauge A/S",
                desc: "2019 - Internship",
              },
              {
                title: "Design Assistant",
                name: "Gift Master",
                desc: "2016 - Internship",
              },
              {
                title: "Design and production manager",
                name: "Garage Culture",
                desc: "2016 - Ongoing",
              },
            ],
          },
          {
            id: 4,
            content: [
              {
                title: "PBA Fashion Design",
                name: "EASV , Soenderborg",
                desc: "September 2013 — January 2018",
              },
              {
                title: "AP Multimedia Design",
                name: "EASV, Esbjerg",
                desc: "2020 - Ongoing",
              },
            
            ],
          },
        ],
      };
    },
  };
</script>
