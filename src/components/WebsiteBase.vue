<template>
  <v-container class="fill-height">
    <v-app-bar style="align-self: center;">
      <v-container>
        <v-row>
          <v-col></v-col>
          <v-col class="flex-grow-1 flex-shrink-0" cols="1" style="max-width:fit-content; min-width: fit-content;">
            <v-app-bar-title d-inline-flex style="max-width: min-content; align-items: center;">{{ pageHeading }}</v-app-bar-title>
          </v-col>
          <v-col></v-col>
        </v-row>
      </v-container>
      <template v-slot:extension style="align-content: center;">
        <v-container>
          <v-row>
            <v-col></v-col>
            <v-col class="flex-grow-1 flex-shrink-0" cols="1" style="max-width:fit-content; min-width: fit-content;">
              <v-tabs
                  show-arrows
                  v-model="tab"
                  align-tabs="center"
                  center-active
                  color="white"
                  height="60"
                  slider-color="white"
                >
                  <v-tab value="0" :text="'Home'"></v-tab>
                  <v-tab value="1" :text="'Photography'"></v-tab>
                  <v-tab value="2" :text="'Posts'"></v-tab>
                  <v-tab value="3" :text="'Experience'"></v-tab>
              </v-tabs>
            </v-col>
            <v-col></v-col>
          </v-row>
        </v-container>  
      </template>
    </v-app-bar>
    <Home v-if="tab == 0"/>
    <Photography v-if="tab == 1"/>
    <Experience v-if="tab == 3"/>
  </v-container>
</template>

<script>

  import Home from './Home.vue'
  import Photography from './Photography.vue'
  import Experience from './Experience.vue'

  export default {
    data() {
      return {
        tab: null,
        pageHeading: 'Silvia Gosálvez Comunión', //homepage
      }
    },

    components: {
      Home,
      Photography,
      Experience,
    }
  }
</script>