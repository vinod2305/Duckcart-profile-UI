<template>
  <v-card outlined class="ma-2">
    <v-list-item class="py-1">
      <span>Evaluation</span>
      <v-spacer></v-spacer>
      <v-btn depressed class="blue--text text--accent-4" color="white">
        <v-icon left>calendar_today</v-icon>SCHEDULE
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn depressed color="white">
        <v-icon>share</v-icon>
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn depressed color="white">
        <v-icon>send</v-icon>
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn depressed  right class="blue--text text--accent-4" color="white">MORE</v-btn>
    </v-list-item>

    <v-divider></v-divider>

    <v-list-item class="py-1">
      <span>Job Name</span>
      <v-spacer></v-spacer>
      <v-btn depressed class="blue--text text--accent-4" color="white">
        <v-icon left>check</v-icon>PROCEED
      </v-btn>
      <v-btn depressed color="white">
        <v-icon>block</v-icon>
      </v-btn>
      <v-btn depressed color="white">
        <v-icon>more_horiz</v-icon>
      </v-btn>
    </v-list-item>

    <v-divider></v-divider>

    <v-list-item class="py-1">
      <span>Pool Name</span>
      <v-spacer></v-spacer>
      <v-btn depressed class="blue--text text--accent-4" color="white">
        <v-icon left>check</v-icon>PROCEED
      </v-btn>
      <v-btn depressed color="white">
        <v-icon>block</v-icon>
      </v-btn>
      <v-btn depressed color="white">
        <v-icon>more_horiz</v-icon>
      </v-btn>
    </v-list-item>
  </v-card>
</template>

<script>
export default {
  data: () => ({})
};
</script>
<style lang="scss" scoped>
.v-card {
  border-radius: 10px;
}
</style>
