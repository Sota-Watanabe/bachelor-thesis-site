<template>
  <section>
    <v-card width="80%" max-width="800" class="mx-auto">
      <div v-for="content in contents" :key="content.title">
        <v-card-title class="headline">
          {{ content.title }}
        </v-card-title>
        <v-card-text>
          <p v-for="paragraph in content.paragraphs" :key="paragraph">
            {{ paragraph }}
          </p>
          <ul v-if="content.items">
            <li v-for="item in content.items" :key="item">
              {{ item }}
            </li>
          </ul>
        </v-card-text>
      </div>
    </v-card>
  </section>
</template>

<script>
export default {
  name: "Overview",
  data: () => ({
    contents: [
      {
        title: "概要",
        paragraphs: [
          "サーバレス実行方式はレイテンシが大きい点が問題となっています。そのレイテンシを小さくするために、先行研究として一定時間コンテナを保持する手法がありますが、非処理時でもメモリを消費するという欠点があります。",
          "本研究ではメモリ量とレイテンシを両方の削減するため、CRIUを使用したコンテナ起動方法を提案しました。コンテナを0から作成し、起動するのではなく,起動済みコンテナのメモリ状態から復元することで初期処理の時間を省くことができます。",
          "この起動方法はすべてのコンテナに有効ではないため、適切なコンテナの条件を実験により明らかにしました。また実用されているソフトウェアでも評価を行い、当該条件が適切であることを確認しました。",
        ],
        items: [],
      },
      {
        title: "成績",
        paragraphs: [],
        items: [
          "芝浦工業大学デザイン工学部総合プロジェクト優秀研究賞を受賞",
          "2020年電子情報通信学会総合大会にて発表",
        ],
      },
    ],
  }),
};
</script>

<style scoped>
section {
  margin: 120px 0;
}
p,
li {
  margin: 0.5rem 0;
  line-height: 1.5rem;
}
li {
  list-style-position: inside;
}
.mx-auto {
  margin: 0 auto;
}
</style>
