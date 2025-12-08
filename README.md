<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>猫カフェ ふにふに</title>

<style>
/* ------------------------------
   全体の基本設定
--------------------------------*/
body {
  margin: 0;
  font-family: "Noto Sans JP", sans-serif;
  color: #444;
  background: #ffffff;
  line-height: 1.7;
}

/* コンテンツを中央に寄せる */
.container {
  width: 90%;
  max-width: 900px;
  margin: auto;
}

/* ------------------------------
   ヒーロー（最上段の大画像）
--------------------------------*/
.hero {
  position: relative;
  text-align: center;
}
.hero img {
  width: 100%;
  height: auto;
  display: block;
}

/* 左上のタイトルボックス */
.hero-title {
  position: absolute;
  top: 20px;
  left: 20px;
  background: #ffe9a9;
  padding: 12px 18px;
  border-radius: 10px;
}
.hero-title h1 {
  margin: 0;
  font-size: 24px;
}

/* ------------------------------
   サブ画像
--------------------------------*/
.showcase img {
  width: 100%;
  border-radius: 16px;
  margin-top: 20px;
}

/* ------------------------------
   ボタンエリア（左端画像 + ボタン）
--------------------------------*/
.menu-block {
  display: flex;
  align-items: flex-start;
  gap: 20px;
  margin-top: 35px;
}

/* 左側の縦画像（btn-side.png） */
.side-img {
  width: 120px;
  height: auto;
  border-radius: 12px;
}

/* ボタンをまとめて並べる領域 */
.menu-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: center;
  flex: 1;
}

/* ボタンスタイル */
.menu-buttons button {
  background: #ffe9a9;
  border: none;
  padding: 12px 20px;
  border-radius: 8px;
  font-size: 15px;
  cursor: pointer;
}

/* スマホ（600px以下）では縦並びにする */
@media (max-width: 600px) {
  .menu-block {
    flex-direction: column;
    align-items: center;
  }
  .side-img {
    width: 60%;
    max-width: 200px;
  }
}

/* ------------------------------
   共通セクション
--------------------------------*/
.section {
  padding: 40px 0;
  text-align: center;
}

/* ------------------------------
   店舗情報
--------------------------------*/
.shop-info img {
  width: 100%;
  border-radius: 16px;
  margin-bottom: 15px;
}
.shop-info-text {
  text-align: left;
  font-size: 15px;
  margin-top: 10px;
}

/* ------------------------------
   料金表
--------------------------------*/
.price-table table {
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  border-collapse: collapse;
}

.price-table th,
.price-table td {
  padding: 12px;
  border-bottom: 1px solid #ddd;
  font-size: 16px;
}

.price-table th {
  background: #ffe9a9;
}

/* ------------------------------
   予約画像
--------------------------------*/
.reserve img {
  width: 100%;
  border-radius: 16px;
  margin-top: 30px;
}

</style>
</head>

<body>

<!-- =========================================
     最上段ヒーロー画像
========================================= -->
<div class="hero">
  <img 
    src="https://github.com/owl-jp-k/cat-cafe4/blob/main/images/main.png?raw=1" 
    alt="猫カフェのメインビジュアル"
  >
  <div class="hero-title">
    <h1>猫カフェ みにふに</h1>
  </div>
</div>


<!-- =========================================
     サブ画像（猫が集まっている写真）
========================================= -->
<div class="showcase container">
  <img 
    src="https://github.com/owl-jp-k/cat-cafe4/blob/main/images/sub.png?raw=1"
    alt="猫たちが集まっている様子"
  >
</div>


<!-- =========================================
     ボタン＋左端画像エリア
========================================= -->
<div class="menu-block container">

  <!-- 左端の縦画像 -->
  <img 
    class="side-img"
    src="https://github.com/owl-jp-k/cat-cafe4/blob/main/images/btn-side.png?raw=1"
    alt="ご利用案内のイメージ画像"
  >

  <!-- ボタン群 -->
  <div class="menu-buttons">
    <button>猫と遊ぶ</button>
    <button>デートのひとときに</button>
    <button>カフェとして</button>
    <button>勉強スペースとして</button>
  </div>

</div>


<!-- =========================================
     店舗情報
========================================= -->
<div class="shop-info container section">
  <img 
    src="https://github.com/owl-jp-k/cat-cafe4/blob/main/images/adress.png?raw=1"
    alt="猫カフェ店舗の外観画像"
  >

  <div class="shop-info-text">
    <p><strong>住所：</strong> 東京都架空市夢町ゆめ通り 0-0-1</p>
    <p><strong>電話番号：</strong> 00-0000-0000</p>
    <p><strong>営業時間：</strong> 10:00〜21:00（最終入店 20:30）</p>
    <p><strong>年中無休：</strong> 1年中いつでも営業中！</p>
  </div>
</div>


<!-- =========================================
     料金表
========================================= -->
<div class="price-table container section">
  <h2>料金</h2>

  <table>
    <tr>
      <th>平日</th>
      <td>¥200（20分）</td>
      <td>¥2,400（3時間）</td>
    </tr>
    <tr>
      <th>休日</th>
      <td>¥250（20分）</td>
      <td>¥2,700（3時間）</td>
    </tr>
  </table>

  <p style="font-size:13px; margin-top:10px;">
    ※延長は10分ごとに ¥350 追加されます
  </p>
</div>


<!-- =========================================
     予約ボタン画像
========================================= -->
<div class="reserve container section">
  <img 
    src="https://github.com/owl-jp-k/cat-cafe4/blob/main/images/btn-reserve.png?raw=1"
    alt="予約はこちらのボタン"
  >
</div>

</body>
</html>
