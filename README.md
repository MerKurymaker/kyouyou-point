# 教養ポイント — ニホンカモシカ協会

友達同士で教養を記録・共有するアプリ。映画・ドラマ・アニメ・本・漫画の消費をポイント化。

## 🚀 デプロイ手順（GitHub Pages）

### 1. GitHubリポジトリ作成
```bash
# 新しいリポジトリを作成（GitHub.comで "kyouyou-point" 等の名前で作成）
# ローカルにclone
git clone https://github.com/YOUR_USERNAME/kyouyou-point.git
cd kyouyou-point
```

### 2. ファイルを配置
以下のファイルをリポジトリのルートにコピー:
- `index.html` — アプリ本体
- `manifest.json` — PWA設定
- `sw.js` — オフライン対応
- `icon-192.png` — アプリアイコン（小）
- `icon-512.png` — アプリアイコン（大）

### 3. GitHubにプッシュ
```bash
git add .
git commit -m "Initial deploy"
git push origin main
```

### 4. GitHub Pages を有効化
1. リポジトリの **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)**
4. **Save**

数分後に `https://YOUR_USERNAME.github.io/kyouyou-point/` で公開される。

### 5. iPhoneにアプリとして追加
1. Safariで上記URLを開く
2. **共有ボタン（□↑）** をタップ
3. **「ホーム画面に追加」** をタップ
4. 完了

→ ホーム画面にカモシカアイコンのアプリが追加される。フルスクリーン・独立アプリとして起動。

## 📱 特徴
- **完全オフライン動作** — Service Workerでキャッシュ
- **Claude不要** — AI API一切不使用。独自レコメンドエンジン
- **データはローカル保存** — localStorageに永続化
- **PWA** — ネイティブアプリのような体験

## ⚙️ カスタマイズ
アプリ内の ⚙️ ボタンから:
- アプリ名変更
- メンバー追加/削除
- 別コミュニティとして複製可能
