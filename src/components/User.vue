<template>
  <v-container>
    <v-row>
      <v-avatar class="mt-2" color="grey" size="130">
        <v-img src="https://cdn.vuetifyjs.com/images/profiles/marcus.jpg"></v-img>
      </v-avatar>
      <div class="ma-3 d-flex flex-column justify-center">
        <p class="display-2 mb-0 title-name">Kamal Pratap</p>
        <p class="headline mb-0 title-detail">full stack developer</p>
        <p class="headline mb-0 title-activity">last activity</p>
      </div>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style lang="scss" scoped>
.title-detail {
  color: #bcbcbc;
}
.title-activity {
  color: #bcbcbc;
}
</style>
