<template>
  <div>
    <v-app-bar app color="primary">
      <div class="d-flex align-center white--text">Real Estate Commerce 24</div>
      <v-spacer class="hidden-xs-only"></v-spacer>
      <v-form>
        <v-autocomplete
          chips
          clearable
          hide-details
          hide-selected
          item-text="name"
          item-value="estate"
          label="Search for a real estate..."
          solo
          class="light-blue lighten-5"
        >
        </v-autocomplete>
      </v-form>
      <v-app-bar-nav-icon class="white--text" @click="drawer = true"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary right>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      group: null,
    };
  },
};
</script>

<style>
</style>