<template>
  <v-card outlined class="ma-0">
    <v-subheader>
      <span class="text--primary subtitle-1">Information</span>
      <v-spacer></v-spacer>
      <v-btn icon color="#404040">
        <v-icon>add_circle_outline</v-icon>
      </v-btn>
    </v-subheader>

    <v-container class="py-1">
      <v-row>
        <v-col :cols="1">
          <span>EMAIL</span>
        </v-col>
        <v-col>
          <span class="value">{{items.email}}</span>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-row>
        <v-col :cols="1">
          <span>PHONE</span>
        </v-col>
        <v-col>
          <span class="value">{{items.phone}}</span>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-row>
        <v-col :cols="1">
          <span>SOCIAL</span>
        </v-col>
        <v-col>
          <span class="value">{{items.social}}</span>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-row>
        <v-col :cols="1">
          <span>LINKS</span>
        </v-col>
        <v-col>
          <div class="value">{{items.links.codepen}}</div>
          <div class="value">{{items.links.yahoo}}</div>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>
<script>
export default {
  data: () => ({
    items: {
      email: "kamalpratap@xyz.com",
      phone: "+91-9876543234",
      social: "github.com/kamalpratap",
      links: {
        codepen: "codepen.io/kamal",
        yahoo: "yahoo.io/kamal"
      }
    },
    model: 1
  })
};
</script>

<style lang="scss" scoped>
.value {
  color: #5f6368;
}
</style>
