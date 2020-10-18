<template>
  <v-app-bar>
    <v-spacer></v-spacer>
    <v-icon style="margin: 10px">mdi-school</v-icon>
    <header>そーたの卒業研究紹介サイト</header>
    <v-avatar size="35" style="margin: 0 10px">
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
