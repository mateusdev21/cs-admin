<template>
  <v-navigation-drawer
    :mini-variant="miniVariant"
    fixed
    app
    style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important"
  >
    <div class="profile" v-if="!miniVariant">
      <div class="profile-pic">
      </div>
      <div class="profile-name">
        <h5>John Doe</h5>
      </div>
    </div>
    <v-avatar size="45" v-if="miniVariant" class="mx-1 mt-2">
      <img
        src="https://img.freepik.com/free-vector/businessman-character-avatar-isolated_24877-60111.jpg?w=826&t=st=1673507251~exp=1673507851~hmac=b83b4e96a9a243a946084088dd29598fbc3d0f3049a5852f5505c00e8e902460"
        width="50"
      />
    </v-avatar>
    <v-list class="px-0">
      <v-list-item
        v-for="(item, i) in sidebarMenu"
        :key="i"
        :to="item.to"
        router
        exact
      >
        <v-list-item-action>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title v-text="item.title" />
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "SideBar",
  props: {
    miniVariant: Boolean,
    sidebarMenu: Array,
  },
  data: () => ({}),
};
</script>

<style lang="scss">
.profile {
  background: url("https://img.freepik.com/free-vector/businessman-character-avatar-isolated_24877-60111.jpg?w=826&t=st=1673507251~exp=1673507851~hmac=b83b4e96a9a243a946084088dd29598fbc3d0f3049a5852f5505c00e8e902460") no-repeat;
  background-position: center;
  background-size: cover;
  .profile-pic {
    padding: 50px 15px;
  }
}
.profile-name {
  background: rgba(0, 0, 0, 0.5);
  h5 {
    padding: 10px;
    color: white;
    text-overflow: ellipsis;
    white-space: nowrap;
    overflow: hidden;
  }
}
.v-list-item--active {
  background: #32c4ce;
  color: white !important;
  opacity: 1;
  .v-avatar {
    color: inherit;
  }
}
</style>
