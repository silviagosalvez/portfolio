
<template>
    <v-container>
      <v-row>
        <v-col style="justify-self: center; align-self: center;">
          {{ "picture here" }}
        </v-col>
        <v-col>
          <div>
            <div class="text-h5">About</div>
            <br><br>
            {{ "description here" }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
    export default {
      props: ['page', 'changePage'],
      methods: {
        projectsClicked() {
          this.$emit('projects', 1)
        }
      }
    }
  </script>
  