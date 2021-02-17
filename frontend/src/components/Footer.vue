<template>
  <v-footer color="grey lighten-3" padless>
    <v-container>
    <v-row no-gutters justify="center">
      <v-col class="my-2 pl-2 ml-4 footer_column" cols="8" md="2">
        <h4 class="font-weight-medium footer_title">Find real estate agent</h4> 
        <v-row no-gutters><v-col>Agent1</v-col></v-row>
        <v-row no-gutters><v-col>Agent2</v-col></v-row>
        <v-row no-gutters><v-col>Agent3</v-col></v-row>
      </v-col>
      <v-col class="my-2 pl-2 ml-4 footer_column" cols="8" md="2">
        <h4 class="font-weight-medium footer_title">Buy and sell residential</h4>
        <v-row no-gutters><v-col>Project sales & rentals</v-col></v-row>
        <v-row no-gutters><v-col>REC24 buyer advice</v-col></v-row>
        <v-row no-gutters><v-col>Parental purchase</v-col></v-row>
      </v-col>
      <v-col class="my-2 pl-2 ml-4 footer_column" cols="8" md="2">
        <h4 class="font-weight-medium footer_title">About the residential market</h4>
        <v-row no-gutters><v-col>Residential news</v-col></v-row>
        <v-row no-gutters><v-col>Subscribe to newsletter</v-col></v-row>
        <v-row no-gutters><v-col>Press</v-col></v-row>
      </v-col>
      <v-col class="my-2 pl-2 ml-4 footer_column" cols="8" md="2">
        <h4 class="font-weight-medium footer_title">About REC24</h4>
        <v-row no-gutters><v-col>About REC24</v-col></v-row>
        <v-row no-gutters><v-col>Job at REC24</v-col></v-row>
        <v-row no-gutters><v-col>Become a franchisee</v-col></v-row>
      </v-col>
    </v-row>
    </v-container>
    <v-container fluid>
      <v-row>
        <v-col class="grey lighten-2 py-4 text-center black--text" cols="12">
        {{ new Date().getFullYear() }} — <strong>Real Estate Commerce 24</strong>
      </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  name: "Footer",
  data() {

  },
};
</script>

<style>
.footer_column {
  border-top: 1px solid #b2aeae;
}

.footer_title {
  font-size: 1.2em;
}
</style>