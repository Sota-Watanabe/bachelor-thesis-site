<template>
  <v-toolbar height="100">
    <v-spacer />
    <!-- class="text-center"が使えない...なぜ -->
    <v-toolbar-title style="text-align: center">
      <nobr
        >サーバレス<wbr />実行方式の<wbr />メモリ消費を<wbr />考慮した<wbr />レイテンシ削減</nobr
      >
    </v-toolbar-title>
    <v-spacer />
  </v-toolbar>
</template>

<script>
export default {
  name: "KeyVisual",

  data: () => ({
    //
  }),
};
</script>

<style scoped>
nobr {
  /* margin: 20px 0 40px; */
  font-size: 32px;
}
</style>
