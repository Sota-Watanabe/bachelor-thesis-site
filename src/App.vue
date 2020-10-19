<template>
  <v-app>
    <Header />
    <KeyVisual />
    <Overview />
    <Documents />
    <Footer />
  </v-app>
</template>

<script>
import Header from "./components/Header";
import KeyVisual from "./components/KeyVisual";
import Overview from "./components/Overview";
import Documents from "./components/Documents";
import Footer from "./components/Footer";

export default {
  name: "App",

  components: {
    Header,
    KeyVisual,
    Overview,
    Documents,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>
