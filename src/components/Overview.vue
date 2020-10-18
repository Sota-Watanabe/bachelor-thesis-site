<template>
  <div style="margin: 120px 0 120px">
    <v-card max-width="800" style="margin: auto">
      <v-card-title class="headline">概要</v-card-title>
      <v-card-text>
        サーバレス実行方式はレイテンシが大きい点が問題となっています。
        そのレイテンシを小さくするために、
        先行研究として一定時間コンテナを保持する手法がありますが、
        非処理時でもメモリを消費するという欠点があります。<br />
        本研究ではメモリ量とレイテンシを両方の削減するため、
        CRIUを使用したコンテナ起動方法を提案しました。コンテナを0から作成し、
        起動するのではなく,
        起動済みコンテナのメモリ状態から復元することで初期処理の時間を省くことができます。<br />
        この起動方法はすべてのコンテナに有効ではないため、
        適切なコンテナの条件を実験により明らかにしました。
        また実用されているソフトウェアでも評価を行い、当該条件が適切であることを確認しました。
      </v-card-text>
      <v-card-title class="headline">成績</v-card-title>
      <v-card-text style="margin: 0 20px">
        <ul>
          <li>芝浦工業大学デザイン工学部総合プロジェクト優秀研究賞を受賞</li>
          <li>2020年電子情報通信学会総合大会にて発表</li>
        </ul>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
  name: "Overview",

  data: () => ({
    //
  }),
};
</script>
