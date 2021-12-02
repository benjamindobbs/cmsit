<template>
  <v-app>
    <v-main>
      <v-layout class="justify-center">
        <nuxt />
        <v-col>
          <v-row  justify="center">
            <h1>Classical Magnet Info Tech</h1>
          </v-row>
          <v-row row d-flex nowrap align="center" justify="center">
              <v-btn 
              rounded
              outlined
              to="/newticket">
                Submit a New Ticket Here
              </v-btn>
          </v-row>
        </v-col>
      </v-layout>
    </v-main>
  </v-app>
</template>
