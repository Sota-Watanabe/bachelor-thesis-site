<template>
  <v-app-bar>
    <v-spacer></v-spacer>
    <v-icon class="mx-4">mdi-school</v-icon>
    <header class="text-center">
      <nobr>そーたの<wbr />卒業研究紹介サイト</nobr>
    </header>
    <v-avatar size="35" class="mx-4">
      <img src="../assets/face_illust.png" alt="Sota" />
    </v-avatar>
    <v-spacer></v-spacer>
  </v-app-bar>
</template>

<script>
export default {
  name: "Header",

  data: () => ({
    //
  }),
};
</script>

<style scoped>
header {
  font-size: 16px;
}
</style>
