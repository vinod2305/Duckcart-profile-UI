<template>
  <nav>
    <v-app-bar flat class="white">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-toolbar-title>
        <span class="font-weight-medium">EMPLOYEES</span>
        /
        <span class="text--secondary">PROFILES</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <span class="font-weight-medium">BACK</span>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title d-flex flex-row align-center ">
            <v-app-bar-nav-icon></v-app-bar-nav-icon>
            <span class="blue--text text--accent-4 pl-3">INOGIT</span>
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list dense nav>
        <v-list-item v-for="item in items1" :key="item.title" link>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-divider></v-divider>
      <v-list dense nav>
        <v-list-item v-for="item in items2" :key="item.title" link>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
    items1: [
      { title: "Dashboard", icon: "dashboard" },
      { title: "Candidates", icon: "supervisor_account" },
      { title: "Jobs", icon: "work" },
      { title: "Mailbox", icon: "chat" },
      { title: "Settings", icon: "settings" },
    ],
    items2: [
      { title: "Pools", icon: "waves" },
      { title: "Assessments", icon: "assessment" },
      { title: "Team Members", icon: "group_work" },
      { title: "Billing", icon: "monetization_on" },
      { title: "Guidelines", icon: "assignment" },
      { title: "Feedback", icon: "feedback" },
      { title: "Contact US", icon: "contact_support" },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>

<style></style>
