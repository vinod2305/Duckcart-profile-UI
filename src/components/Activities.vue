<template >
  <v-container class="pa-0">
    <v-row>
      <v-col class="pl-4 pt-2">
        <Information />
      </v-col>
    </v-row>
    <v-row>
      <v-col class="pl-4 pt-1">
        <Experience />
      </v-col>
    </v-row>
    <v-row align-content="stretch" align="stretch">
      <v-col class="pl-4 pt-1" align-self="stretch">
        <Education />
      </v-col>
      <v-col class="pl-4 pt-1 " align-self="stretch">
        <Skills />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Education from "./Activity/Education";
import Experience from "./Activity/Experience";
import Information from "./Activity/Information";
import Skills from "./Activity/Skills";

export default {
  components: {
    Education,
    Experience,
    Information,
    Skills
  },
  data: () => ({})
};
</script>
