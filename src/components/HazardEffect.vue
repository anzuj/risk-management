<template>
  <v-card color="grey lighten-4" class="mt-4 pa-4">
    <h3 class="ml-8">Hazard Effects reference</h3>

    <v-row>
      <v-col>
        <v-card flat height="100%">
          <v-card-text>
            <b
              >S Severity <br />
              (Hazard Effect / Impact) <br />
              →
            </b>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col v-for="effect in effects" :key="effect.text">
        <v-card flat :color="effect.color" height="100%">
            <!-- <v-sheet color="black" class="py-1">
<p class="text-center white--text">{{effect.icon}}</p>
            </v-sheet> -->
          <v-card-text class="d-flex">
        
   <v-avatar size="45" color="black" class="white--text mr-2" 
              >{{effect.icon}}</v-avatar
            >
        
         
            <div>{{effect.text}}</div>
          </v-card-text>
        </v-card>
      </v-col>
  
    </v-row>
  </v-card>
</template>

<script>
export default {
  props: [""],
  components: {},
  data: () => ({
    effects: [
      {
        icon: "VH",
        color: "#E54120",
        text: "Death, system loss, severe financial loss",
      },
      {
        icon: "H",
        color: "#F36C35",
        text:
          "High – Irrecoverable severe injury / illness, major system damage, major financial loss",
      },
      {
        icon: "M",
        color: "yellow",
        text:
          "Moderate – Irrecoverable light injury / illness, moderate system damage, small financial loss",
      },
      {
        icon: "L",
        color: "#C4DD36",
        text:
          "Low – Recoverable light injury /illness, small system damage, small financial loss",
      },
      {
        icon: "VL",
        color: "#8BCC1B",
        text:
          "Very Low – Will not result in injury /illness, nearly no system damage, small financial loss",
      },
    ],
    probabilities: [],
  }),
  methods: {},
  computed: {},
};
</script>
