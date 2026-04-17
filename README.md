# ✝ バイブルドッヂ - ダビデ vs ゴリアテ

聖句の真偽を見抜いて戦う、ドッジボール×聖書クイズゲーム。

![ダビデ vs ゴリアテ](assets/images/background.jpg)

## 遊び方

1. `index.html` をブラウザで開く
2. 🔊ボタンをタップして音楽ON
3. 「戦いを始める」で対戦開始

## ルール

- ターン開始時、ダビデとゴリアテが掛け合いをする
- ボールを投げる時、聖句を叫ぶ
- 受ける側は **〇(本物)** か **×(偽物)** で判定
- **正解**でボールを避ける → 相手に **10ダメージ** (反撃)
- **判定ミス** → 自分が **CRITICAL 40ダメージ** を受ける
- 先に相手のHPをゼロにしたら勝利

## 特徴

- 🎭 ダビデとゴリアテの本格アニメキャラクター
- 💬 ターン毎に異なる掛け合いセリフ
- 🎵 Sunoで作曲したオリジナルBGM + 勝利賛美歌
- 🔥 ドラゴンボール風のチャージオーラ演出
- 💥 CRITICAL時は派手に吹っ飛ぶ
- 🪨 ダビデは石投げ名手なので投石のように飛ぶ
- 📖 **口語訳聖書**を使用、本物43種・偽物28種を収録

## ファイル構成

```
.
├── index.html              # ゲーム本体
├── README.md
└── assets/
    ├── images/
    │   ├── david.png       # ダビデのキャラクター画像
    │   ├── goliath.png     # ゴリアテのキャラクター画像
    │   └── background.jpg  # エラの谷の戦場背景
    └── audio/
        ├── title.mp3       # タイトル画面BGM
        ├── battle.mp3      # バトルBGM
        ├── victory.mp3     # 勝利ジングル/賛美歌
        └── defeat.mp3      # 敗北ジングル
```

## GitHub Pagesで公開する

1. リポジトリの **Settings → Pages**
2. **Source**: `Deploy from a branch`
3. **Branch**: `main` / `/ (root)` → Save
4. 数分後 `https://<ユーザー名>.github.io/<リポジトリ名>/` で公開

## ローカルで試す

```bash
cd bible-dodge
python3 -m http.server 8000
# または
npx http-server
```

ブラウザで `http://localhost:8000` を開く。

## クレジット

- キャラクターデザイン: Midjourney
- BGM/賛美歌: Suno AI
- ゲーム開発: Claude (Anthropic)
