<template>
  <v-app>
    <Navbar />
    <v-container fluid class="py-0">
      <v-row>
        <v-col :cols="8" class="pa-2">
          <v-card class="`d-flex flex-column`" flat tile>
            <User />
            <Tabs class="mt-3"/>
          </v-card>
        </v-col>
        <v-col :cols="4" class="pa-2">
          <v-card class="`d-flex flex-column`" flat tile>
            <Utilities />
            <Teamnotes />
            <Tasks />
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import Navbar from "./components/Navbar";
import User from "./components/User";
import Tabs from "./components/Tabs";
import Teamnotes from "./components/Teamnotes";
import Tasks from "./components/Tasks";
import Utilities from "./components/Utilities";
export default {
  components: {
    Navbar,
    User,
    Tabs,
    Teamnotes,
    Tasks,
    Utilities
  },
  name: "App",
  data() {
    return {};
  }
};
</script>
