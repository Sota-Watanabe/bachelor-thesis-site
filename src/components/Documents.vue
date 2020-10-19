<template>
  <div class="text-center">
    <v-toolbar flat prominent max-width="1000" class="mx-auto">
      <v-tabs v-model="tabs" center-active center fixed-tabs show-arrows>
        <!-- <v-tab href="#tab-1">総合大会用の梗概(1ページ)</v-tab> -->
        <v-tab href="#tab-2">最終発表の梗概</v-tab>
        <v-tab href="#tab-4">卒業論文</v-tab>
        <v-tab href="#tab-3">最終発表の資料</v-tab>
      </v-tabs>
    </v-toolbar>
    <v-tabs-items v-model="tabs">
      <v-tab-item value="tab-1" style="height: 100vh">
        <iframe
          width="85%"
          height="100%"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/ieice-synopsis.pdf"
        ></iframe>
      </v-tab-item>
      <v-tab-item value="tab-2" style="height: 100vh">
        <iframe
          width="85%"
          height="100%"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/synopsis.pdf"
        ></iframe>
      </v-tab-item>
      <v-tab-item value="tab-3" style="height: 100vh">
        <iframe
          src="https://onedrive.live.com/embed?resid=EF9A5F5BC26C037%2121277&amp;authkey=%21AFMwpXu8ZSYzNzg&amp;em=2&amp;wdAr=1.3333333333333333"
          width="100%"
          height="500"
          frameborder="0"
          >これは、<a target="_blank" href="https://office.com/webapps"
            >Office</a
          >
          の機能を利用した、<a target="_blank" href="https://office.com"
            >Microsoft Office</a
          >
          の埋め込み型のプレゼンテーションです。</iframe
        >
      </v-tab-item>
      <v-tab-item value="tab-4" style="height: 100vh">
        <iframe
          width="80%"
          height="100%"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/thesis.pdf#page=1"
        ></iframe>
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
export default {
  name: "Documents",

  data: () => ({
    tabs: "tab-1",
  }),
};
</script>

<style scoped>
/* iframe */
</style>
