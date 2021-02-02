<template>
  <v-footer color="grey lighten-3" padless>
    <v-row no-gutters>
      <v-col text class="my-2 pl-4" 
        ><span class="font-weight-medium">Find real estate agent</span> 
        <v-row no-gutters><v-col>Agent1</v-col></v-row>
        <v-row no-gutters><v-col>Agent2</v-col></v-row>
        <v-row no-gutters><v-col>Agent3</v-col></v-row>
      </v-col>
      <v-col text class="my-2 pl-2"
        ><span class="font-weight-medium">Buy and sell residential</span>
        <v-row no-gutters><v-col>Project sales & rentals</v-col></v-row>
        <v-row no-gutters><v-col>REC24 buyer advice</v-col></v-row>
        <v-row no-gutters><v-col>Parental purchase</v-col></v-row>
      </v-col>
      <v-col text class="my-2 pl-2"
        ><span class="font-weight-medium">News about the residential market</span>
        <v-row no-gutters><v-col>Residential news</v-col></v-row>
        <v-row no-gutters><v-col>Subscribe to newsletter</v-col></v-row>
        <v-row no-gutters><v-col>Press</v-col></v-row>
      </v-col>
      <v-col text class="my-2 pl-2"
        ><span class="font-weight-medium">About REC24</span>
        <v-row no-gutters><v-col>About REC24</v-col></v-row>
        <v-row no-gutters><v-col>Job at REC24</v-col></v-row>
        <v-row no-gutters><v-col>Become a franchisee</v-col></v-row>
      </v-col>
      <v-col class="grey lighten-2 py-4 text-center black--text" cols="12">
        {{ new Date().getFullYear() }} — <strong>Real Estate Commerce 24</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data() {

  },
};
</script>

<style>
</style>