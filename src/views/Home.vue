<template>
  <v-container>
    <h1 class="text-center mb-5 d-none">
      <v-icon color="indigo">mdi-card-bulleted-outline</v-icon> Awesome risk management portal
    </h1>
    <v-card class="mx-auto pa-6" min-height="600">
      <v-row class="">
        <v-spacer></v-spacer>
        <v-btn
          fab
          dark
          color="indigo darken-3"
          large
          title="create new project"
          @click="createRisk = !createRisk"
        >
          <v-icon large>{{ createRisk ? "mdi-minus" : "mdi-plus" }}</v-icon>
        </v-btn>
      </v-row>

      <v-expand-transition>
        <v-row v-if="createRisk" class="mt-3">
          <CreateRisk />
        </v-row>
      </v-expand-transition>
    </v-card>
  </v-container>
</template>

<script>
import CreateRisk from "@/components/CreateRisk.vue";
export default {
  props: [""],
  components: { CreateRisk },
  data: () => ({
    createRisk: true,
  }),
  methods: {},
  computed: {},
};
</script>
