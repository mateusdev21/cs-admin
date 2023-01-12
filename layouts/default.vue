<template>
  <v-app>
    <ToolBar class="toolbar" @toggle-mini="miniVariant = !miniVariant" />
    <v-main>
      <SideBar
        class="sidebar"
        :miniVariant="miniVariant"
        :sidebarMenu="sidebarMenu"
      />
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import SideBar from "~/components/SideBar.vue";
import ToolBar from "~/components/ToolBar.vue";
export default {
  name: "DefaultLayout",
  components: {
    ToolBar,
    SideBar,
  },
  data() {
    return {
      fixed: false,
      sidebarMenu: [
        {
          title: "Dashboard",
          icon: "mdi-view-dashboard-outline",
          to: "/",
        },
        {
          title: "Alerts",
          icon: "mdi-alert-circle-outline",
          to: "/alerts",
        },
        {
          title: "Buttons",
          icon: "mdi-radiobox-blank",
          to: "/components-testing/buttons",
        },
        {
          title: "Cards",
          icon: "mdi-card-outline",
          to: "/cards",
        },
        {
          title: "Carousel",
          icon: "mdi-form-dropdown",
          to: "/carousel",
        },
        {
          title: "Tables",
          icon: "mdi-table",
          to: "/tables",
        },
      ],
      miniVariant: false,
      title: "Vuetify.js",
    };
  },
};
</script>

<style>
.v-main__wrap {
  background-color: #eef5f9;
  padding-top: 10vh;
  padding-left: 2vw;
  padding-right: 2vw;
}
.sidebar {
  z-index: 1004 !important;
  margin-top: 64px;
}
.toolbar {
  z-index: 1006 !important;
}
</style>
