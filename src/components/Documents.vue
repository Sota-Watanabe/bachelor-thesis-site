<template>
  <div class="text-center my-12">
    <v-toolbar prominent>
      <v-tabs v-model="tab" center-active center fixed-tabs show-arrows>
        <v-tabs-slider></v-tabs-slider>
        <v-tab v-for="item in items" :key="item">
          {{ item }}
        </v-tab>
      </v-tabs>
    </v-toolbar>
    <v-tabs-items v-model="tab">
      <v-tab-item v-for="element in elements" :key="element">
        <v-card height="100vh" class="py-16" prominent>
          <iframe width="85%" height="100%" frameborder="0" v-bind:src="element" />
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
export default {
  name: "Documents",

  data: () => ({
    tab: null,
    items: ["梗概", "卒業論文", "発表資料"],
    elements: [
      "https://thesis-documents.s3-ap-northeast-1.amazonaws.com/synopsis.pdf",
      "https://thesis-documents.s3-ap-northeast-1.amazonaws.com/thesis.pdf",
      "https://onedrive.live.com/embed?resid=EF9A5F5BC26C037%2121277&authkey=%21AFMwpXu8ZSYzNzg&em=2&wdAr=1.3333333333333333",
    ],
  }),
};
</script>

<style scoped>
</style>
