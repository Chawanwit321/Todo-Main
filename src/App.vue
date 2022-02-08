<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://i.pinimg.com/736x/7c/09/48/7c0948ac69a90aac021fe06632e5a667.jpg"
          transition="scale-transition"
          width="95"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn to="/"  text>
        <span class="mr-2">Home</span>
      </v-btn>
       <v-btn to="/about"  text>
        <span class="mr-2">about</span>
      </v-btn>
       <v-btn to="/Todo"  text>
        <span class="mr-2">Todo</span>
      </v-btn>
    </v-app-bar>
    

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
