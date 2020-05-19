<template>
  <v-card outlined class="ma-0 rounded-card" height="100%">
    <v-list flat>    
    <v-subheader>
        <span class="text--primary subtitle-1">Skils</span>
        <v-spacer></v-spacer>
        <v-btn icon color="#404040">
          <v-icon>add_circle_outline</v-icon>
        </v-btn>
      </v-subheader>
    <v-list-item class="ml-5">
      <v-chip-group column>
        <v-chip 
          color="#E3F2FD"
          class="black--text  text--primary px-6 ma-1 skills-chip"
          v-for="(tag, i) in tags"
          :key="i"
        >{{ tag }}</v-chip>
      </v-chip-group>
    </v-list-item>
    </v-list>
  </v-card>
</template>
<script>

export default {
  data: () => ({
    tags: [
      "Python",
      "Web Development",
      "CSS",
      "Web Development",
      "Python",
      "CSS",
      "CSS",
      "Web Development",
      "Python",
      "Web Development",
      "Python",
      "CSS",
      "CSS",
      "Web Development",
      "Python"
    ]
  })
};
</script>

<style lang="scss" scoped>
.rounded-card{
    border-radius:8px !important;
}
</style>
