<template>
  <v-app dark>
    <v-tabs centered>
      <v-tab
        v-for="(item, i) in items"
        :key="i"
        :to="item.to"
        nuxt
        router
        exact
      >
        {{ item.title }}
      </v-tab>
    </v-tabs>
    <v-spacer />
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
        {
          icon: "mdi-format-list-checks",
          title: "Ticket Queue",
          to: "/ticketqueue",
        },
      ],
      title: "Classical Magnet IT",
    };
  },
};
</script>
