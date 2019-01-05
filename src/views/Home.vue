<template>
  <div class="home">
    <v-parallax dark src="https://cdn.vuetifyjs.com/images/parallax/material.jpg">
      <v-layout align-center column justify-center>
        <h1 class="display-2 font-weight-thin mb-3">ITF Attendance Manager</h1>
        <v-btn class="mt-4" depressed large color="white" href="settings">getting start</v-btn>
        <v-btn
          outline
          depressed
          large
          color="white"
          href="https://community.vuetifyjs.com"
          target="_blank"
        >Github Page</v-btn>
      </v-layout>
    </v-parallax>
    <homebody/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import homebody from "@/components/homebody.vue"; // @ is an alias to /src

@Component({
  components: {
    homebody
  }
})
export default class Home extends Vue {}
</script>
