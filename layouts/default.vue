<template>
  <v-app>
    <v-tabs centered fixed-tabs>
      <v-tab
        v-for="(item, i) in items"
        :key="i"
        :to="item.to"
        nuxt
        router
      >
        {{ item.title }}
      </v-tab>
    </v-tabs>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          icon: "mdi-home-outline",
          title: "Welcome",
          to: "/",
        },
        {
          icon: "mdi-archive-plus-outline",
          title: "Create Ticket",
          to: "/newticket",
        },
        {icon: "mdi-archive-plus-outline",
          title: "Create Student Ticket",
          to: "/newStudentTicket",
        },
        {
          icon: "mdi-format-list-checks",
          title: "Ticket Queue",
          to: "/ticketqueue",
        },
        {
          icon: "",
          title: "FAQ",
          to: "/faq"
        },
        {
          icon:"",
          title:"Tutorials",
          to:"/tutorials"
        }
      ],
      title: "Classical Magnet IT",
    };
  },
};
</script>
