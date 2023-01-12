<template>
    <div class="continer container-fluid">
        <v-card style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important" class="mb-8">
            <v-card-title class="px-6">Square Buttons</v-card-title>
            <v-divider></v-divider>
            <v-card-text>
                <ButtonSquare dark color="primary" class="mx-2" label="Primary"/>
                <ButtonSquare dark color="secondary" class="mx-2" label="Secondary"/>
                <ButtonSquare dark color="success" class="mx-2" label="Success"/>
                <ButtonSquare dark color="warning" class="mx-2" label="Warning"/>
                <ButtonSquare dark color="error" class="mx-2" label="Error"/>
                <ButtonSquare class="mx-2" label="Normal"/>
                <ButtonSquare disabled class="mx-2" label="Disabled"/>
            </v-card-text>
        </v-card>
        <v-card style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important" class="mb-8">
            <v-card-title class="px-6">Outlined Buttons</v-card-title>
            <v-divider></v-divider>
            <v-card-text>
                <ButtonSquare outlined color="primary" class="mx-2" label="Primary"/>
                <ButtonSquare outlined color="secondary" class="mx-2" label="Secondary"/>
                <ButtonSquare outlined color="success" class="mx-2" label="Success"/>
                <ButtonSquare outlined color="warning" class="mx-2" label="Warning"/>
                <ButtonSquare outlined color="error" class="mx-2" label="Error"/>
                <ButtonSquare outlined class="mx-2" label="Normal"/>
                <ButtonSquare outlined disabled class="mx-2" label="Disabled"/>
            </v-card-text>
        </v-card>
        <v-card style="box-shadow: 0px 1px 10px rgba(0, 0, 0, 0.34) !important" class="mb-8">
            <v-card-title class="px-6">Buttons With Icon</v-card-title>
            <v-divider></v-divider>
            <v-card-text>
                <ButtonSquare icon="mdi-face-agent" color="primary" class="mx-2" label="Primary"/>
                <ButtonSquare icon="mdi-face-agent" color="secondary" class="mx-2" label="Secondary"/>
                <ButtonSquare icon="mdi-face-agent" color="success" class="mx-2" label="Success"/>
                <ButtonSquare icon="mdi-face-agent" color="warning" class="mx-2" label="Warning"/>
                <ButtonSquare icon="mdi-face-agent" color="error" class="mx-2" label="Error"/>
                <ButtonSquare icon="mdi-face-agent" class="mx-2" label="Normal"/>
                <ButtonSquare icon="mdi-face-agent" disabled class="mx-2" label="Disabled"/>
            </v-card-text>
        </v-card>
    </div>
</template>

<script>
import ButtonSquare from "~/components/Buttons/ButtonSquare.vue"
export default {
    name: "Buttons",
    components: {
        ButtonSquare,
    }
}
</script>