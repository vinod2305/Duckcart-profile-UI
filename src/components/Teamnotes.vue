<template>
  <v-card outlined class="ma-2 my-3">
    <v-list :two-line="twoLine" :nav="nav" :avatar="avatar" class="pa-0">
      <v-subheader>
        <span class="text--primary subtitle-1">Team Notes</span>
        <v-spacer></v-spacer>
        <v-btn icon color="#404040">
          <v-icon>add_circle_outline</v-icon>
        </v-btn>
      </v-subheader>
      <v-list-item-group v-model="item">
        <v-list-item v-for="(item, i) in items" :key="i" inactive>
          <v-avatar color="#2962FF" size="40" class="mx-2">
            <span class="white--text">KP</span>
          </v-avatar>
          <v-list-item-content class="pa-1">
            <v-list-item-title class="my-1">
              <span>{{item.title}}</span>
              •
              <span class="text--secondary caption">{{item.time}}</span>
            </v-list-item-title>
            <v-list-item-subtitle v-html="item.subtitle" class="mt-1 mb-3"></v-list-item-subtitle>

            <v-divider v-show="i < '3'"></v-divider>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-card>
</template>





<script>
export default {
  data: () => ({
    item: 4,
    items: [
      {
        title: "Kamal Pratap",
        time: "02:30 pm",
        subtitle: "Hey Guys, i've pushed my progress to the Master Branch"
      },
      {
        title: "Kamal Pratap",
        time: "02:30 pm",
        subtitle: "Hey Guys, i've pushed my progress to the Master Branch"
      },
      {
        title: "Kamal Pratap",
        time: "02:30 pm",
        subtitle: "Hey Guys, i've pushed my progress to the Master Branch"
      },
      {
        title: "Kamal Pratap",
        time: "02:30 pm",
        subtitle: "Hey Guys, i've pushed my progress to the Master Branch"
      }
    ],
    twoLine: true,
    nav: true,
    avatar: true,
    rounded: true
  })
};
</script>
