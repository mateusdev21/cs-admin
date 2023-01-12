<template>
  <div class="continer container-fluid">
    <v-row class="mb-8">
      <v-card
        style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important"
        width="100%"
      >
        <v-card-title class="px-6">Square Buttons</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonSquare
            dark
            color="primary"
            class="mx-2 text-capitalize"
            label="Primary"
          />
          <ButtonSquare
            dark
            color="secondary"
            class="mx-2 text-capitalize"
            label="Secondary"
          />
          <ButtonSquare
            dark
            color="success"
            class="mx-2 text-capitalize"
            label="Success"
          />
          <ButtonSquare
            dark
            color="warning"
            class="mx-2 text-capitalize"
            label="Warning"
          />
          <ButtonSquare
            dark
            color="error"
            class="mx-2 text-capitalize"
            label="Error"
          />
          <ButtonSquare class="mx-2 text-capitalize" label="Normal" />
          <ButtonSquare
            disabled
            class="mx-2 text-capitalize"
            label="Disabled"
          />
        </v-card-text>
      </v-card>
    </v-row>
    <v-row class="mb-8">
      <v-card
        style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important"
        width="100%"
      >
        <v-card-title class="px-6">Outlined Buttons</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonSquare
            outlined
            color="primary"
            class="mx-2 text-capitalize"
            label="Primary"
          />
          <ButtonSquare
            outlined
            color="secondary"
            class="mx-2 text-capitalize"
            label="Secondary"
          />
          <ButtonSquare
            outlined
            color="success"
            class="mx-2 text-capitalize"
            label="Success"
          />
          <ButtonSquare
            outlined
            color="warning"
            class="mx-2 text-capitalize"
            label="Warning"
          />
          <ButtonSquare
            outlined
            color="error"
            class="mx-2 text-capitalize"
            label="Error"
          />
          <ButtonSquare outlined class="mx-2 text-capitalize" label="Normal" />
          <ButtonSquare
            outlined
            disabled
            class="mx-2 text-capitalize"
            label="Disabled"
          />
        </v-card-text>
      </v-card>
    </v-row>
    <v-row class="mb-8">
      <v-card
        style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important"
        width="100%"
      >
        <v-card-title class="px-6">Buttons With Icon</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonSquare
            icon="mdi-face-agent"
            color="primary"
            class="mx-2 text-capitalize"
            label="Primary"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            color="secondary"
            class="mx-2 text-capitalize"
            label="Secondary"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            color="success"
            class="mx-2 text-capitalize"
            label="Success"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            color="warning"
            class="mx-2 text-capitalize"
            label="Warning"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            color="error"
            class="mx-2 text-capitalize"
            label="Error"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            class="mx-2 text-capitalize"
            label="Normal"
          />
          <ButtonSquare
            icon="mdi-face-agent"
            disabled
            class="mx-2 text-capitalize"
            label="Disabled"
          />
        </v-card-text>
      </v-card>
    </v-row>
    <v-row class="d-flex justify-space-between mb-8">
      <v-card width="32%">
        <v-card-title class="px-6">Block Button</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonSquare
            dark
            block
            color="primary"
            label="Primary"
            class="mb-4 text-capitalize"
          />
          <ButtonSquare
            dark
            block
            color="secondary"
            label="Secondary"
            class="mb-4 text-capitalize"
          />
        </v-card-text>
      </v-card>
      <v-card width="32%">
        <v-card-title class="px-6">Icon Button</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonIcon icon="mdi-home" color="primary" class="mx-2" />
          <ButtonIcon
            icon="mdi-refresh-circle"
            color="secondary"
            class="mx-2"
          />
          <ButtonIcon icon="mdi-check-circle" color="success" class="mx-2" />
          <ButtonIcon icon="mdi-alert" color="warning" class="mx-2" />
          <ButtonIcon icon="mdi-alert-circle" color="error" class="mx-2" />
          <ButtonIcon icon="mdi-account-circle" class="mx-2" />
          <ButtonIcon icon="mdi-lock" disabled class="mx-2" />
        </v-card-text>
      </v-card>
      <v-card width="32%">
        <v-card-title>Rounded Button</v-card-title>
        <v-divider></v-divider>
        <v-card-text>
          <ButtonSquare
            dark
            rounded
            color="primary"
            class="mx-2 mb-4 text-capitalize"
            label="Primary"
          />
          <ButtonSquare
            dark
            rounded
            color="secondary"
            class="mx-2 mb-4 text-capitalize"
            label="Secondary"
          />
          <ButtonSquare
            dark
            rounded
            color="success"
            class="mx-2 mb-4 text-capitalize"
            label="Success"
          />
          <ButtonSquare
            dark
            rounded
            color="warning"
            class="mx-2 mb-4 text-capitalize"
            label="Warning"
          />
          <ButtonSquare
            dark
            rounded
            color="error"
            class="mx-2 mb-4 text-capitalize"
            label="Error"
          />
          <ButtonSquare rounded class="mx-2 mb-4 text-capitalize" label="Normal" />
          <ButtonSquare
            disabled
            rounded
            class="mx-2 mb-4 text-capitalize"
            label="Disabled"
          />
        </v-card-text>
      </v-card>
    </v-row>
  </div>
</template>

<script>
import ButtonSquare from "~/components/Buttons/ButtonSquare.vue";
import ButtonIcon from "~/components/Buttons/ButtonIcon.vue";
export default {
  name: "Buttons",
  components: {
    ButtonSquare,
    ButtonIcon,
  },
};
</script>
