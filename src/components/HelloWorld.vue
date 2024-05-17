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
                  v-model="tab"
                  align-tabs="center"
                  color="white"
                  height="60"
                  slider-color="#f78166"
                >
                  <v-tab>Home</v-tab>
                  <v-tab>Photography</v-tab>
              </v-tabs>
            </v-col>
            <v-col></v-col>
          </v-row>
        </v-container>  
      </template>
    </v-app-bar>
  </v-container>
</template>

<script>

  import Home from './Home.vue'

  export default {
    // Properties returned from data() become reactive state
    // and will be exposed on `this`.
    data() {
      return {
        page: 0, //homepage
        pageHeading: 'Silvia Gosalvez' //homepage
      }
    },

    // Methods are functions that mutate state and trigger updates.
    // They can be bound as event handlers in templates.
    methods: {
      changePage(page) {
        let initialPage = this.page
        this.page = page;
        this.pageHeading = this.page == 0 ? 'Taylor Stevens' : this.page == 1 ? 'Projects' : this.page == 2 ? 'Contact Me' : 'Unknown Page'
        this.$forceUpdate();
        console.log(`recieved page change from ${initialPage} to page ${page}`)
      },
    },

    components: {
      Home,
    }
  }
</script>