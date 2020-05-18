<template>
  <v-card outlined class="tab-box">
    <v-tabs v-model="tab">
      <v-tab v-for="item in items" :key="item.tab">{{ item.tab }}</v-tab>
    </v-tabs>
    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item.tab">
        <v-card flat >
          <v-card-text class="pa-0">
            <component  v-bind:is="item.content"></component>
          </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
import Overview from "./Overview";
import Activities from "./Activities";
import Assessments from "./Assessments";
import Files from "./Files";
import Resume from "./Resume";
export default {
  components: {
    Overview,
    Activities,
    Assessments,
    Files,
    Resume
  },
  data: () => ({
    tab: null,
    items: [
      { tab: "overview", content: "Overview" },
      { tab: "activities", content: "Activities" },
      { tab: "assessments", content: "Assessments" },
      { tab: "files", content: "Files" },
      { tab: "resume", content: "Resume" }
    ]
  })
};
</script>

<style lang="scss" scoped>
.tab-box {
  border: none !important;
}
</style>
