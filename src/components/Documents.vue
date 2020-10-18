<template>
  <div>
    <v-tabs v-model="model">
      <v-tab href="#tab-1">総合大会用の梗概(1ページ)</v-tab>
      <v-tab href="#tab-2">最終発表用の梗概(2ページ)</v-tab>
      <v-tab href="#tab-3">最終発表の資料</v-tab>
      <v-tab href="#tab-4">卒業論文</v-tab>
    </v-tabs>
    <v-tabs-items v-model="model">
      <v-tab-item value="tab-1">
        <iframe
          width="100%"
          height="1200"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/ieice-synopsis.pdf"
        ></iframe>
      </v-tab-item>
      <v-tab-item value="tab-2">
        <iframe
          width="100%"
          height="1200"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/synopsis.pdf"
        ></iframe>
      </v-tab-item>
      <v-tab-item value="tab-3">
        <iframe
          src="https://onedrive.live.com/embed?resid=EF9A5F5BC26C037%2121277&amp;authkey=%21AFMwpXu8ZSYzNzg&amp;em=2&amp;wdAr=1.3333333333333333"
          width="350px"
          height="286px"
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
      <v-tab-item value="tab-4">
        <iframe
          width="100%"
          height="1200"
          src="https://thesis-documents.s3-ap-northeast-1.amazonaws.com/thesis.pdf"
        ></iframe>
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>

<script>
export default {
  name: "Documents",

  data: () => ({
    model: "tab-1",
  }),
};
</script>
