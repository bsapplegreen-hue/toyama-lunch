<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>富山旅行 2日目ランチ候補リスト</title>
  <style>
    :root {
      --primary: #2d6a4f;
      --bg: #f4f6f8;
      --card-bg: #ffffff;
      --text: #2b2b2b;
      --accent: #e76f51;
      --badge-bg: #e8f5e9;
      --badge-text: #1b5e20;
    }
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      background-color: var(--bg);
      color: var(--text);
      margin: 0;
      padding: 12px;
      padding-bottom: 40px;
    }
    header {
      text-align: center;
      padding: 10px 0 12px;
    }
    h1 {
      font-size: 1.25rem;
      margin: 0 0 4px;
      color: var(--primary);
    }
    p.sub {
      font-size: 0.8rem;
      color: #666;
      margin: 0 0 12px;
    }
    /* 検索バー */
    .search-box {
      margin-bottom: 12px;
    }
    .search-input {
      width: 100%;
      padding: 10px 14px;
      border: 1px solid #ccc;
      border-radius: 20px;
      font-size: 0.85rem;
      box-sizing: border-box;
      outline: none;
    }
    /* タブ切り替えボタン */
    .tabs {
      display: flex;
      overflow-x: auto;
      gap: 6px;
      padding-bottom: 8px;
      margin-bottom: 12px;
      -webkit-overflow-scrolling: touch;
    }
    .tab-btn {
      background: #e0e0e0;
      border: none;
      padding: 8px 12px;
      border-radius: 20px;
      font-size: 0.8rem;
      white-space: nowrap;
      cursor: pointer;
      font-weight: bold;
      color: #555;
    }
    .tab-btn.active {
      background: var(--primary);
      color: #fff;
    }
    /* 見出し */
    .sec-title {
      font-size: 0.95rem;
      margin-bottom: 10px;
      padding-left: 8px;
      border-left: 4px solid var(--primary);
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-weight: bold;
    }
    /* カードデザイン */
    .tab-content { display: none; }
    .tab-content.active { display: block; }
    .card {
      background: var(--card-bg);
      border-radius: 12px;
      padding: 14px;
      margin-bottom: 12px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.05);
    }
    .card-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 4px;
    }
    .shop-name {
      font-weight: bold;
      font-size: 1.05rem;
      color: #1a1a1a;
      text-decoration: none;
    }
    .rating {
      color: #f39c12;
      font-weight: bold;
      font-size: 0.88rem;
      white-space: nowrap;
    }
    .review-count {
      font-size: 0.75rem;
      color: #888;
      font-weight: normal;
    }
    /* アクセス・エリアタグ */
    .meta-info {
      display: flex;
      flex-wrap: wrap;
      gap: 4px;
      margin: 6px 0 8px;
    }
    .tag {
      font-size: 0.72rem;
      padding: 3px 8px;
      border-radius: 4px;
      background: #f0f0f0;
      color: #444;
    }
    .tag.area {
      background: var(--badge-bg);
      color: var(--badge-text);
      font-weight: bold;
    }
    .tag.access {
      background: #e3f2fd;
      color: #0d47a1;
    }
    .description {
      font-size: 0.83rem;
      line-height: 1.45;
      color: #555;
      margin: 0 0 10px;
    }
    /* アクションボタン */
    .btn-group {
      display: flex;
      gap: 8px;
    }
    .action-btn {
      flex: 1;
      text-align: center;
      padding: 6px 0;
      font-size: 0.75rem;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }
    .btn-map {
      background: #eaf4fe;
      color: #1a73e8;
      border: 1px solid #d2e3fc;
    }
    .btn-nav {
      background: var(--primary);
      color: #fff;
    }
  </style>
</head>
<body>

<header>
  <h1>🍽️ 富山ガチ旨ランチ候補</h1>
  <p class="sub">Google評価 ★4.0以上限定リスト</p>
</header>

<!-- 絞り込み検索 -->
<div class="search-box">
  <input type="text" id="searchInput" class="search-input" placeholder="🔍 エリア名（例：高岡、砺波、氷見）で絞り込み..." onkeyup="filterShops()">
</div>

<!-- タブボタン -->
<div class="tabs">
  <button class="tab-btn active" onclick="openTab(event, 'soba')">🍜 そば・うどん</button>
  <button class="tab-btn" onclick="openTab(event, 'ramen')">🍜 富山ブラック</button>
  <button class="tab-btn" onclick="openTab(event, 'western')">🍽️ レストラン・洋食</button>
  <button class="tab-btn" onclick="openTab(event, 'kaiten')">🍣 回転寿司</button>
  <button class="tab-btn" onclick="openTab(event, 'sushi')">🍣 回らないお寿司</button>
</div>

<!-- 1. そば・うどん -->
<div id="soba" class="tab-content active">
  <div class="sec-title">そば・うどん <span>6軒</span></div>
  
  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">手打ちうどん どんたく</span>
      <span class="rating">★4.4 <span class="review-count">(602件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜15分</span>
      <span class="tag access">⛰️ 相倉〜50分</span>
    </div>
    <p class="description">出汁の旨味が抜群。サクサクのカツが乗った「カツカレーうどん」や天ぷらが地元で圧倒的人気。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=手打ちうどん+どんたく+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=手打ちうどん+どんたく+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">手打ちうどん 田じま</span>
      <span class="rating">★4.3 <span class="review-count">(78件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜25分</span>
      <span class="tag access">⛰️ 相倉〜40分</span>
    </div>
    <p class="description">のどかなエリアにある綺麗な古民家風。モチモチの太麺とうどんを覆う大きな海老天が好評。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=手打ちうどん+田じま+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=手打ちうどん+田じま+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="砺波市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">御食事処 尾の上</span>
      <span class="rating">★4.2 <span class="review-count">(162件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 砺波市</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜30分</span>
    </div>
    <p class="description">地元に根付いた和食の老舗。名物「割子そば」や衣が軽くて美味しい天ぷらが愛されている。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=御食事処+尾の上+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=御食事処+尾の上+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="南砺市 城端 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">ヨッテカーレ城端 むぎや</span>
      <span class="rating">★4.1 <span class="review-count">(420件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 南砺市(城端)</span>
      <span class="tag access">🌊 雨晴〜45分</span>
      <span class="tag access">⛰️ 相倉〜20分</span>
    </div>
    <p class="description">SA直結で一般道からも入れる。富山名物「白エビ天うどん」や、注文後に握る熱々のおにぎりが大好評。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=ヨッテカーレ城端+むぎや" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=ヨッテカーレ城端+むぎや" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="南砺市 城端 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">手打そば 萱笑</span>
      <span class="rating">★4.1 <span class="review-count">(501件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 南砺市(城端)</span>
      <span class="tag access">🌊 雨晴〜40分</span>
      <span class="tag access">⛰️ 相倉〜25分</span>
    </div>
    <p class="description">地元南砺産の石臼挽き二八そば。頭までサクサク食べられる大きな天然エビ天ぷらの満足度が高い。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=手打そば+萱笑+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=手打そば+萱笑+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">うどん・そば 今庄 高岡駅南店</span>
      <span class="rating">★4.0 <span class="review-count">(550件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">高岡市民のソウルフード。早い・安い・旨いが揃い、うどんとそばを1つの器に混ぜた「ちゃんぽん」が名物。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=うどん・そば+今庄+高岡駅南店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=うどん・そば+今庄+高岡駅南店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>
</div>

<!-- 2. 富山ブラック -->
<div id="ramen" class="tab-content">
  <div class="sec-title">富山ブラックラーメン <span>4軒</span></div>
  
  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">らぁめん次元</span>
      <span class="rating">★4.1 <span class="review-count">(1047件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市(駅前)</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">真っ黒な見た目なのに、焦がし醤油のコクと出汁が効いて「スープまで美味しく飲める」マイルドな黒醤油。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=らぁめん次元+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=らぁめん次元+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">めん八 御旅屋店</span>
      <span class="rating">★4.1 <span class="review-count">(282件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">高岡の夜の街を支えるローカルな名店。スープのパンチと、口の中でとろける分厚いチャーシューが絶品。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=めん八+御旅屋店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=めん八+御旅屋店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">らーめん 翔龍</span>
      <span class="rating">★4.0 <span class="review-count">(1000件超)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜18分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">ローカル番組でも常に上位の高岡を代表する大行列店。旨味が溶け込んだ深い醤油スープと中太ちぢれ麺。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=らーめん+翔龍+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=らーめん+翔龍+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">らーめん 誠や</span>
      <span class="rating">★4.0 <span class="review-count">(839件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜22分</span>
      <span class="tag access">⛰️ 相倉〜40分</span>
    </div>
    <p class="description">コショウがガツンと効いた、元祖に近い味。何よりうどん並みに太くコシの強い「極太ちぢれ麺」が熱狂的人気。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=らーめん+誠や+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=らーめん+誠や+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>
</div>

<!-- 3. レストラン・洋食 -->
<div id="western" class="tab-content">
  <div class="sec-title">レストラン・洋食 <span>6軒</span></div>
  
  <div class="card" data-keywords="南砺市 井波 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">Cucina Nobu</span>
      <span class="rating">★4.2 <span class="review-count">(113件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 南砺市(井波)</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜30分</span>
    </div>
    <p class="description">築100年の伝統古民家を改装。隠し味に塩麹を使った、薪窯焼きのモチモチピッツァや旬のパスタが絶品。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=Cucina+Nobu+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=Cucina+Nobu+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="砺波市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">自由ELE（ジュエル）</span>
      <span class="rating">★4.1 <span class="review-count">(193件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 砺波市</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜30分</span>
    </div>
    <p class="description">ブランド肉「A5ランク氷見牛＆富山ポーク」を使用。肉汁がジュワッと溢れ出す絶品手作りハンバーグ。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=自由ELE+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=自由ELE+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="砺波市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">田園の食卓 ノエル</span>
      <span class="rating">★4.1 <span class="review-count">(371件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 砺波市</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜30分</span>
    </div>
    <p class="description">田んぼに囲まれたのどかな一軒家。卵がとろとろでデミグラスソースが美味しい「スペシャルオムライス」が定番。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=田園の食卓+ノエル+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=田園の食卓+ノエル+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">キャセロール</span>
      <span class="rating">★4.1 <span class="review-count">(280件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">長年愛される高岡の老舗洋食店。特製デミグラスソースがグツグツと煮立った鉄鍋の「煮込みハンバーグ」が有名。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=キャセロール+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=キャセロール+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">雨晴ベイサイドカフェ</span>
      <span class="rating">★4.0 <span class="review-count">(20件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市(雨晴)</span>
      <span class="tag access">🌊 雨晴〜1分</span>
      <span class="tag access">⛰️ 相倉〜55分</span>
    </div>
    <p class="description">雨晴海岸が目の前という抜群のオーシャンビュー。綺麗な器で提供される本格パスタやカツカレー。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=雨晴ベイサイドカフェ" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=雨晴ベイサイドカフェ" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="砺波市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">ビストロ ブランシュ</span>
      <span class="rating">★4.0 <span class="review-count">(74件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 砺波市</span>
      <span class="tag access">🌊 雨晴〜30分</span>
      <span class="tag access">⛰️ 相倉〜35分</span>
    </div>
    <p class="description">砺波市のアットホームなフレンチ。地元食材をふんだんに使い、お箸で気軽に食べられるカジュアルなコースが高コスパ。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=ビストロ+ブランシュ+砺波" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=ビストロ+ブランシュ+砺波" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>
</div>

<!-- 4. 回転寿司 -->
<div id="kaiten" class="tab-content">
  <div class="sec-title">回転寿司 <span>5軒</span></div>
  
  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">すし食いねぇ! 高岡南店</span>
      <span class="rating">★4.1 <span class="review-count">(1000件超)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜25分</span>
      <span class="tag access">⛰️ 相倉〜40分</span>
    </div>
    <p class="description">氷見・金沢港から1日2回直送される圧倒的なネタの鮮度と、大満足できるお値打ちなランチセット。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=すし食いねぇ!+高岡南店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=すし食いねぇ!+高岡南店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">氷見回転寿司 粋鮨 高岡店</span>
      <span class="rating">★4.1 <span class="review-count">(448件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">氷見漁港で競り落とされた地物ネタが自慢。氷見の旬を盛り込んだ「にぎりランチ」の圧倒的なコスパが支持。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=氷見回転寿司+粋鮨+高岡店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=氷見回転寿司+粋鮨+高岡店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="氷見市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">氷見きときと寿し 氷見本店</span>
      <span class="rating">★4.1 <span class="review-count">(2000件超)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 氷見市</span>
      <span class="tag access">🌊 雨晴〜15分</span>
      <span class="tag access">⛰️ 相倉〜55分</span>
    </div>
    <p class="description">県外からもファンが集まる有名チェーンの総本店。白エビ天ぷらやホタルイカなど、富山湾名物の質の高さ。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=氷見きときと寿し+氷見本店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=氷見きときと寿し+氷見本店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">番やのすし 高岡店</span>
      <span class="rating">★4.0 <span class="review-count">(920件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">富山県民の満足度が非常に高いローカルチェーン。他店よりさらに希少な地魚ネタが安く回る穴場。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=番やのすし+高岡店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=番やのすし+高岡店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">廻る富山湾 すし玉 高岡店</span>
      <span class="rating">★4.0 <span class="review-count">(640件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜25分</span>
      <span class="tag access">⛰️ 相倉〜40分</span>
    </div>
    <p class="description">毎朝セリ落とされる地物11貫の「富山湾盛り」や、無料サービスでもらえる「かわはぎの味噌汁」が地元密着で人気。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=廻る富山湾+すし玉+高岡店" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=廻る富山湾+すし玉+高岡店" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>
</div>

<!-- 5. 回らないお寿司 -->
<div id="sushi" class="tab-content">
  <div class="sec-title">回らないお寿司（5,000円以下） <span>8軒</span></div>
  
  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">富山湾氷見前鮨 銀兆</span>
      <span class="rating">★4.8 <span class="review-count">(35件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市(戸出)</span>
      <span class="tag access">🌊 雨晴〜30分</span>
      <span class="tag access">⛰️ 相倉〜35分</span>
    </div>
    <p class="description">伝統工芸「能作」の錫の器で味わう上質な空間。贅沢な「富山湾鮨ランチ」が3,600円で楽しめる。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=富山湾氷見前鮨+銀兆" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=富山湾氷見前鮨+銀兆" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">亀寿し</span>
      <span class="rating">★4.7 <span class="review-count">(185件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">地元の食通が通うカウンター寿司。富山湾の最高な海の幸10貫セットが2,500円という驚異の神コスパ。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=亀寿し+富山" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=亀寿し+富山" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="小矢部市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">すし処さかた</span>
      <span class="rating">★4.5 <span class="review-count">(62件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 小矢部市</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜35分</span>
    </div>
    <p class="description">小矢部市の地域密着店。1,000円〜2,000円台で驚くほど豪華な寿司ランチや海鮮丼が食べられる。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=すし処さかた+小矢部" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=すし処さかた+小矢部" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">大黒鮨</span>
      <span class="rating">★4.5 <span class="review-count">(55件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市</span>
      <span class="tag access">🌊 雨晴〜22分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">高岡の住宅街の超穴場。メニューなし、大将おまかせ9貫がなんと2,200円。人情味溢れるローカルな雰囲気が最高。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=大黒鮨+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=大黒鮨+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="高岡市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">鮨金</span>
      <span class="rating">★4.5 <span class="review-count">(168件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 高岡市(駅前)</span>
      <span class="tag access">🌊 雨晴〜20分</span>
      <span class="tag access">⛰️ 相倉〜45分</span>
    </div>
    <p class="description">高岡駅前の実力派老舗。お昼にはカウンターで1,500円から味わえる超お得なランチがあり気楽に入れる。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=鮨金+高岡" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=鮨金+高岡" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="氷見市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">松葉寿司</span>
      <span class="rating">★4.5 <span class="review-count">(209件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 氷見市</span>
      <span class="tag access">🌊 雨晴〜15分</span>
      <span class="tag access">⛰️ 相倉〜55分</span>
    </div>
    <p class="description">落ち着いた佇まいの老舗。白エビを盛り込んだ特製セットが2,500円と非常に良心的。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=松葉寿司+氷見" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=松葉寿司+氷見" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="氷見市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">鮨処 きよ水</span>
      <span class="rating">★4.3 <span class="review-count">(182件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 氷見市(漁港前)</span>
      <span class="tag access">🌊 雨晴〜15分</span>
      <span class="tag access">⛰️ 相倉〜55分</span>
    </div>
    <p class="description">氷見漁港の目の前。あら汁や茶碗蒸しが付く特上ランチが2,300円。漁港前ならではの圧倒的な鮮度。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=鮨処きよ水+氷見" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=鮨処きよ水+氷見" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>

  <div class="card" data-keywords="砺波市 雨晴 相倉">
    <div class="card-header">
      <span class="shop-name">幸ずし（となみ幸ずし）</span>
      <span class="rating">★4.0 <span class="review-count">(46件)</span></span>
    </div>
    <div class="meta-info">
      <span class="tag area">📍 砺波市</span>
      <span class="tag access">🌊 雨晴〜35分</span>
      <span class="tag access">⛰️ 相倉〜30分</span>
    </div>
    <p class="description">砺波駅近く。美しい器で出てくる「富山湾鮨（3,000円）」の満足度が高く、今回のルート上で最も立ち寄りやすい。</p>
    <div class="btn-group">
      <a class="action-btn btn-map" href="https://www.google.com/maps/search/?api=1&query=となみ幸ずし" target="_blank">🔍 Googleマップ</a>
      <a class="action-btn btn-nav" href="https://www.google.com/maps/dir/?api=1&destination=となみ幸ずし" target="_blank">🚗 ナビ開始</a>
    </div>
  </div>
</div>

<script>
  function openTab(evt, tabId) {
    const contents = document.querySelectorAll('.tab-content');
    contents.forEach(content => content.classList.remove('active'));
    
    const buttons = document.querySelectorAll('.tab-btn');
    buttons.forEach(btn => btn.classList.remove('active'));
    
    document.getElementById(tabId).classList.add('active');
    evt.currentTarget.classList.add('active');
    
    // タブ切り替え時に検索を再適用
    filterShops();
  }

  function filterShops() {
    const input = document.getElementById('searchInput').value.toLowerCase();
    const cards = document.querySelectorAll('.card');
    
    cards.forEach(card => {
      const text = card.textContent.toLowerCase() + " " + (card.getAttribute('data-keywords') || "");
      if (text.includes(input)) {
        card.style.display = "";
      } else {
        card.style.display = "none";
      }
    });
  }
</script>

</body>
</html>
