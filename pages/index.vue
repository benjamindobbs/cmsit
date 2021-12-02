<template>
  <v-app>
    <v-main>
      <v-container fill-height>
        <v-layout>
          <nuxt />
          <h1>Classical Magnet Info Tech</h1>
          <v-btn
          to='/newticket'
          >
          Submit a New Ticket Here
          </v-btn>
          <v-btn
          to='/ticketqueue'
          >
          See the Ticket Queue
          </v-btn>
        </v-layout>
      </v-container>
    </v-main>
  </v-app>
</template>
