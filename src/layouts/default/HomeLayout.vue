<template>
  <v-layout>
    <!-- <v-system-bar color="deep-purple darken-3"></v-system-bar> -->
    <v-app-bar flat style="background-color: #1a3c59; color: white">
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-toolbar-title>
        <span class="mr-2"><v-icon icon="mdi-twitter"></v-icon></span>
        <span class="ml-4"><v-icon icon="mdi-email-outline"></v-icon></span>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>

      <v-text-field
        label="search"
        prepend-inner-icon="mdi-map-marker"
        variant="solo"
        class=""
        style="height:10px; position:relative; top:-22px"
      ></v-text-field>

      <v-btn variant="text" class="text-capitalize">monthly bulletin</v-btn>
      <hr />
      <v-btn variant="text">news & insights</v-btn>

      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
    </v-app-bar>
    <!--  -->
    <v-app-bar prominent>
      <v-app-bar-nav-icon
        variant="text"
        @click.stop="drawer = !drawer"
        class="d-flex d-sm-none"
      ></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-toolbar-title class="pt-2">
        <img src="/logo.jpeg" style="width: 70px" />
      </v-toolbar-title>

      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
      <div class="me-5">
        <v-btn variant="text">our story</v-btn>

        <v-btn variant="text">what we do</v-btn>

        <v-btn variant="text">news & insights</v-btn>

        <v-btn variant="text">jurisdictions</v-btn>

        <v-btn variant="text">careers </v-btn>
        <v-btn variant="text">stay connected </v-btn>
      </div>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>
    </v-app-bar>
    <!-- mobile drawer -->
    <v-navigation-drawer v-model="drawer" location="bottom" temporary>
      <v-list :items="items"></v-list>
    </v-navigation-drawer>

    <v-main style="height: 500px">
      <!-- banner image -->
      <div class="container">
        <img
          src="https://media.istockphoto.com/id/1207994690/photo/cyborg-hand-pressing-a-keyboard-on-a-laptop-in-dark-blue-background-3d-rendering.jpg?s=612x612&w=0&k=20&c=SbMfg-z3guMjDpvq3Dbz6l-UyT3kgRAWnCugmTJg3qw="
          alt="Snow"
          style="width: 100%; height: 900px"
        />

        <div class="centered homeFont font-weight-bold text-left">
          <div>welcome to the World of IP</div>

          <div class="text-center centered-button">
            <v-btn
              variant="tonal"
              class="button font-weight-bold text-capitalize"
            >
              learn more
            </v-btn>
          </div>
        </div>
        <!-- banner image ends here -->
      </div>
      <router-view></router-view>
      <br />
      <br />
      <!-- footer -->
      <Footer></Footer>
      <!--  -->
    </v-main>
  </v-layout>
</template>

<script>
import Footer from "../../components/Footer";
export default {
  components: {
    Footer,
  },
  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: "Foo",
        value: "foo",
      },
      {
        title: "Bar",
        value: "bar",
      },
      {
        title: "Fizz",
        value: "fizz",
      },
      {
        title: "Buzz",
        value: "buzz",
      },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
