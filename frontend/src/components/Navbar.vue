<template>
  <div>
    <v-app-bar app color="red darken-4">
      <v-toolbar-title class="white--text"><router-link
          to="/"
          class="white--text logotext"
          title="Real Estate Commerce 24"
          >Real Estate Commerce 24</router-link>
      </v-toolbar-title>
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
          class="light-red lighten-5 mr-3"
          color="red darken-4"
        >
        </v-autocomplete>
      </v-form>
      <v-app-bar-nav-icon
        class="white--text"
        @click="drawer = true"
      ></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary right>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-red--text text--accent-4"
        >
          <v-list-item v-for="item in menu" :to="item.route" :key="item.title">
            <v-list-item-icon>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      drawer: false,
      group: null,
      menu: [
        { icon: "mdi-home", title: "Home", route: "/" },
        { icon: "mdi-home-search", title: "Search residential", route: "2" },
        { icon: "mdi-account-search", title: "Find real estate agent", route: "2" },
        { icon: "mdi-home-plus", title: "Buy residential", route: "2" },
        { icon: "mdi-home-minus", title: "Sell residential", route: "2" },
        { icon: "mdi-home-group", title: "Projectsales & rentals", route: "2" },
        { icon: "mdi-cash-multiple", title: "Condos", route: "2" },
        { icon: "mdi-new-box", title: "News about the market", route: "2" },
        { icon: "mdi-information", title: "About REC24", route: "About" },
        { icon: "mdi-home-modern", title: "Homes for rent", route: "2" },
        { icon: "mdi-login", title: "Login REC24", route: "2" },
        { icon: "mdi-account-group", title: "Book free sales assessment", route: "2" },
      ],
    };
  },
};
</script>

<style>
.logotext {
  text-decoration: none;
  font-size: 1.4em;
}
</style>