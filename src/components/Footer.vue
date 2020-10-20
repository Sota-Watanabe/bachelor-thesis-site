<template>
  <v-footer padless class="mt-16">
    <v-card flat tile class="text-center" width="100%">
      <v-divider></v-divider>
      <v-card-text>
        <v-btn
          v-for="link in links"
          :key="link"
          class="mx-4"
          icon
          v-bind:href=link.url
        >
          <v-icon size="24px">
            {{ link.icon }}
          </v-icon>
        </v-btn>
      </v-card-text>
      <v-card-text class="">
        Copyright©{{ new Date().getFullYear() }} — Sota Watanabe.
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: "Footer",

  data: () => ({
    links: [
      {url: "https://thesis.so-ta.net", icon: "mdi-home"},
      {url: "https://portfolio.so-ta.net", icon: "mdi-human-greeting"},
      {url: "https://github.com/sota-watanabe", icon: "mdi-github"},
      {url: "https://twitter.com/Sota___Watanabe", icon: "mdi-twitter"},
    ]
  }),
};
</script>

<style scoped></style>
