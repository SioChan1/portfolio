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
                    <router-link to="/service"
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
                desc: "Familiar and mastered most of the programs.",
              },
              {
                title: "Forcasting",
                name: "Trend analazys",
                desc: "Fashion studies baground and intership experience in trendforcasting, using pantone method",
              },
              {
                title: "Project managment",
                
                desc: "Experience in project managment.",
              },
            ],
          },
          {
            id: 2,
            content: [
              {
                title: "Stuborn",
                name: "Will not stop untill found a sulution to a problem",
                
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
                name: "Will always find a way to listen and understand, both in profesional enviroment and personal.",
                
              },
              {
                title: "Caring",
                name: "Never find it a problem or hard to help out others.",
                
              },
            ],
          },
          {
            id: 3,
            content: [
              {
                title: "Designer Assistent",
                name: "Marc Lauge A/S",
                desc: "2019 - Internship",
              },
              {
                title: "Designer Assistent",
                name: "Gift Master",
                desc: "2016 - Internship",
              },
              {
                title: "Designer and production manager",
                name: "Garage Culture",
                desc: "2016 - ongoing",
              },
            ],
          },
          {
            id: 4,
            content: [
              {
                title: "PBA Fasion Desing",
                name: "EASV , Soenderborg",
                desc: "September 2013 — January 2018",
              },
              {
                title: "AP Multiedia Desing",
                name: "EASV, Esbjerg",
                desc: "2020 - ongoing",
              },
            
            ],
          },
        ],
      };
    },
  };
</script>
