<template>
  <v-app>
    <v-main>
      <v-parallax src="parallax.jpg">
      <v-layout fill-height fluid>
        <v-container fill-height fluid align-items="top">
          <nuxt />
          <v-col
          align-self="center"
          height=100%>
              <v-card
              shaped
              max-width="500"
              > <v-card-text class=text-center> <h1 style="color:black"> Classical Magnet Info Tech</h1> </v-card-text>
              </v-card>
                <v-btn 
                rounded
                to="/newticket"
                color="success">
                  Submit a New Ticket Here
                </v-btn>
                <v-btn 
                rounded
                to="/newStudentTicket"
                color="success">
                  Submit a New Student Ticket Here
                </v-btn>
              
          </v-col>
        </v-container>
      </v-layout>
      </v-parallax>
    </v-main>
  </v-app>
</template>
<script>
export default {
  data() {
    return {
      image: { backgroundImage: "url(/9k.png)" },
    };
  },
};
</script>
