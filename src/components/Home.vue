
<template>
    <v-container>
      <v-row>
        <v-col style="justify-self: center; align-self: center;">
          <v-img
          justify="center"
          class="bg-white rounded-xl"
          width="300"
          :aspect-ratio="1"
          src="./me.jpeg"
          cover
        ></v-img>
        </v-col>
        <v-col>
          <div>
            <div class="text-h5">About</div>
            <br><br>
            My name is Taylor Stevens and I am a Software Engineer with a degree in Computer Science concentrated in Artificial 
            Intelligence from Northeastern University. I have a diverse background with full-stack development where I have worked
            with tools from React and Linux to Nginx and Pyspark. Driven from a passion for public service and mutual aid, I have worked 
            on a range of projects that given me experience in complex problem-solving, leadership, and collaboration.
            <br><br>
            One project that I am particularly proud of is the FosteredFood project, a mutual aid initiative that focuses on reducing food 
            waste and increasing food access for low-income and food-insecure individuals. As the project lead, I have been able to expand 
            and develop my skills in project management and community outreach as well as my technical skills with Typescript, React, Google 
            API's, and more. 
            <br><br>
            My personal interests include playing rugby as a wing, going bouldering indoors and outdoors, and hiking and camping in the White 
            Mountains in New Hampshire.
            <br><br>
            To explore some of my projects, click here: 
            <v-btn @click="projectsClicked" color="deep-purple-accent-4" flat density="compact">Projects</v-btn>
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
  