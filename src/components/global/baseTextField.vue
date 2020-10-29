<template>
        <!-- v-model="name" -->
  <v-text-field
        class="mb-2"
        hide-details
        filled
        background-color="white"
        :label="label"
        :prepend-icon="icon"
      ></v-text-field>
</template>

<script>
export default {
  props: ["label", "icon"],
  components: {},
  data: () => ({
    name,
  }),
  methods: {},
  computed: {},
};
</script>
