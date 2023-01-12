<template>
  <v-btn
    :rounded="rounded"
    :block="block"
    :depressed="depressed"
    :outlined="outlined"
    :dark="dark"
    :disabled="disabled"
    :color="color"
    :customClass="customClass"
    @click="$emit('onClick')"
  >
    {{ label }}
    <v-icon right dark v-if="icon"> {{ icon }} </v-icon>
  </v-btn>
</template>

<script>
export default {
  name: "ButtonSquare",
  props: {
    rounded: Boolean,
    block: Boolean,
    depressed: Boolean,
    outlined: Boolean,
    dark: Boolean,
    disabled: Boolean,
    color: String,
    customClass: String,
    label: String,
    icon: String,
  },
};
</script>
