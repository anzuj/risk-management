<template>
  <v-container>
    <h2 class="mb-3">Create new project</h2>
    <v-card color="grey lighten-4" class="pa-4">
      <h3 class="ml-8">Basics</h3>
      <v-row>
        <v-col>
          <baseTextField
            :label="'Project name'"
            :icon="'mdi-folder-edit-outline'"
          />
          <baseTextField
            :label="'Customer name'"
            :icon="'mdi-account-hard-hat'"
          />
          <baseTextField :label="'Location'" :icon="'mdi-earth'" />
        </v-col>

        <v-col>
          <baseTextField
            :label="'Evatherm Project No.'"
            :icon="'mdi-folder-information-outline'"
          />
          <baseTextField :label="'Team'" :icon="'mdi-account-group'" />
          <baseTextField
            :label="'In charge'"
            :icon="'mdi-account-star-outline'"
          />
        </v-col>
      </v-row>
    </v-card>

<!-- SPECIFICS -->
        <v-card color="#F7EFEB" class="mt-4 pa-4">
      <h3 class="ml-8">Specifics</h3>
      <v-row>
        <v-col>
         <baseTextField
        :label="'Relevant Engineering Documents'"
        :icon="'mdi-folder-cog-outline'"
      />
        </v-col>

        <v-col>
   
      <baseTextField
        :label="'Medium / Equipment'"
        :icon="'mdi-car-turbocharger'"
      />
        </v-col>
      </v-row>
    </v-card>


    <HazardEffect/>
  </v-container>
  <!-- <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        /> -->
</template>

<script>
import baseTextField from "@/components/global/baseTextField.vue";
import HazardEffect from "@/components/HazardEffect.vue";
export default {
  components: { baseTextField, HazardEffect },
  data: () => ({}),
};
</script>
