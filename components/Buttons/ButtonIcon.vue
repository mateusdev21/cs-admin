<template>
  <v-btn icon :color="color" :disabled="disabled">
    <v-icon>{{ icon }}</v-icon>
  </v-btn>
</template>
<script>
export default {
  name: "ButtonIcon",
  props: {
    color: String,
    icon: String,
    disabled: Boolean,
  },
};
</script>
