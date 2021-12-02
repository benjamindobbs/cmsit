<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          @click.stop="miniVariant = true"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon
        @click.stop="
          () => {
            if ((miniVariant=false) || (drawer=false)) {
              drawer = !drawer;
            } else {
              drawer = true;
            }
            miniVariant = false;
          }
        "
      />
      <v-toolbar-title v-text="title" />
      <v-spacer />
    </v-app-bar>
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
      clipped: true,
      drawer: true,
      fixed: false,
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
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Classical Magnet IT",
    };
  },
};
</script>
