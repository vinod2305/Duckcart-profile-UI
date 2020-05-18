<template>
  <v-card outlined class="ma-2 my-3">
    <v-list flat :two-line="twoLine" :nav="nav" :avatar="avatar" class="pa-0">
      <v-subheader>
        <span class="text--primary subtitle-1">Tasks</span>
        <v-spacer></v-spacer>
        <v-btn icon color="#404040">
          <v-icon>add_circle_outline</v-icon>
        </v-btn>
      </v-subheader>
      <v-list-item-group v-model="item">
        <div v-for="(item, i) in items" :key="i">
          <v-list-item flat inactive class="ma-0">
            <v-list-item-content class="pa-1">
              <v-list-item-title>
                <v-list-item-action class="ma-1">
                  <v-checkbox v-model="item.active" color="primary"></v-checkbox>
                </v-list-item-action>
                <span>{{item.title}}</span>
              </v-list-item-title>
              <v-list-item-subtitle class="mb-3 ml-1 font-weight-medium">
                <span>{{item.update}} </span>•
                <v-icon class="calendar-today">calendar_today</v-icon>
                <span >DUE : </span>
                <span>{{item.time}} </span>
                <span>{{item.date}}</span>
              </v-list-item-subtitle>
            </v-list-item-content>

            <v-list-item-action>
              <v-avatar color="#2962FF" size="35" class="mx-2">
                <span class="white--text">KP</span>
              </v-avatar>
            </v-list-item-action>
          </v-list-item>
          <v-divider></v-divider>
        </div>
      </v-list-item-group>
    </v-list>
  </v-card>
</template>




<script>
export default {
  data: () => ({
    item: 6,
    items: [
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
      {
        title: "Add checkout button",
        time: "03:00pm",
        update: "2MIN AGO",
        date: "02/05/2020",
        active: true
      },
     
    ],
    twoLine: true,
    nav: true,
    avatar: true,
    rounded: true
  })
};
</script>

<style lang="scss" scoped>
.calendar-today {
  font-size: 14px;
  transform: translateY(-2px);
}
</style>