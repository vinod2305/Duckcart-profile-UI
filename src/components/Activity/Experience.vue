<template>
  <v-card outlined class="ma-0 rounded-card">
    <v-subheader>
      <span class="text--primary subtitle-1">Experience</span>
      <v-spacer></v-spacer>
      <v-btn icon color="#404040">
        <v-icon>add_circle_outline</v-icon>
      </v-btn>
    </v-subheader>
    <v-list flat class="pa-0">
      <v-list-item-group>
        <v-list-item v-for="(item, i) in items" :key="i">
          <v-list-item-content class="pt-0 pb-5">
            <v-list-item-title>{{item.role}}</v-list-item-title>
            <v-list-item-subtitle>
              <p class="ma-0">{{item.company}}</p>
              <p class="ma-0">{{item.term}}</p>
              <p class="my-1">{{item.job}}</p>
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-card>
</template>
<script>
export default {
  data: () => ({
    items: [
      {
        role: "Lead Designer",
        company: "Google. Inc.",
        term: "Sep 2019 - Dec 2019",
        job:
          "During my intership, I developed UI and UX for an android app called Google Keep. I completely Re-Designed the application."
      }
    ]
  })
};
</script>
<style lang="scss" scoped>
.rounded-card{
    border-radius:8px !important;
}
</style>