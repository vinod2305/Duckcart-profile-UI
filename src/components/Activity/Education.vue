<template>
  <v-card outlined class="ma-0" height="100%">
    <v-subheader>
      <span class="text--primary subtitle-1">Education</span>
      <v-spacer></v-spacer>
      <v-btn icon color="#404040">
        <v-icon>add_circle_outline</v-icon>
      </v-btn>
    </v-subheader>
    <v-list flat class="pa-0 mb-4">
      <v-list-item-group>
        <v-list-item v-for="(item, i) in items" :key="i">
          <v-list-item-content>
            <v-list-item-title>{{item.qualification}}</v-list-item-title>
            <v-list-item-subtitle>
              <p class="ma-0">{{item.school}}</p>
              <p class="ma-0">{{item.year}}</p>
              <p class="my-1">{{item.grades}}</p>
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
        qualification: "SSC",
        school: "St. Mary High School",
        year: "Sep 2016",
        grades: "CGPA : 9.2"
      },
      {
        qualification: "Higher Secondary",
        school: "St. Mary High School",
        year: "Sep 2018",
        grades: "Percentage : 96.5%"
      }
    ]
  })
};
</script>
