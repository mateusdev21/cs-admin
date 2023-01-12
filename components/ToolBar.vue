<template>
  <v-app-bar elevation="0" color="primary" dark fixed>
    <div class="pe-5">
      <NuxtLink to="/" class="d-flex align-center mb-0">
        <v-icon style="font-size: 2rem; font-weight: 700" class="px-4"
          >mdi-face-agent</v-icon
        >
        <p
          style="color: white; font-size: 1.5rem; font-weight: 700"
          class="mt-4"
        >
          CS-Admin
        </p>
      </NuxtLink>
    </div>
    <v-icon @click.stop="$emit('toggle-mini')" style="font-size: 2rem; font-weight: 700">mdi-backburger</v-icon>
    <v-spacer />
    <v-menu nudge-bottom origin="auto" min-width="300">
      <template v-slot:activator="{ on }">
        <v-btn
          v-on="on"
          class="d-flex align-center pa-0 px-1"
          elevation="0"
          color="transparent"
          plain
          :ripple="false"
        >
          <v-avatar size="35" color="white">
            <img src="https://img.freepik.com/free-vector/businessman-character-avatar-isolated_24877-60111.jpg?w=826&t=st=1673507251~exp=1673507851~hmac=b83b4e96a9a243a946084088dd29598fbc3d0f3049a5852f5505c00e8e902460" width="50"/>
          </v-avatar>
          <p style="color:white" class="my-2 ml-2">John Doe</p>
        </v-btn>
      </template>

      <v-list class="pa-6" elevation="10">
        <v-list-item-group v-model="selectedItem" color="primary">
          <v-list-item two-line v-for="(item, i) in userMenus" :key="i">
            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
              <v-list-item-subtitle>{{ item.desc }}</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
          <v-btn block color="secondary" variant="tonal" class="mt-4 py-4"
            >Logout</v-btn
          >
        </v-list-item-group>
      </v-list>
    </v-menu>
  </v-app-bar>
</template>

<script>
export default {
  name: "ToolBar",
  data: () => ({
    drawer: false,
    userMenus: [
      {
        title: "My Profile",
        desc: "Account Settings",
      },
      {
        title: "My Inbox",
        desc: "Messages & Emails",
      },
      {
        title: "My Tasks",
        desc: "To-do and Daily Tasks",
      },
    ],
    selectedItem: null,
  }),
};
</script>
