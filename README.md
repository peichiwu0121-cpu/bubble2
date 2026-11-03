# 🧋 珍奶打地鼠

一個純 HTML / CSS / JavaScript 的小遊戲，無需安裝任何套件、無需建置，開啟 `index.html` 就能玩。

## 玩法
- 30 秒內敲擊洞裡冒出來的東西
- 🧋 +1、🍰 +2、🌟 +3、💣 −3
- 最高分會存在瀏覽器的 localStorage

## 本機執行
直接用瀏覽器開啟 `index.html`，或：

```bash
python3 -m http.server 8000
```

## 上傳到 GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<你的帳號>/bubble-tea-whack.git
git push -u origin main
```

## 部署到 Cloudflare Pages
1. 登入 Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**
2. 選擇你的 GitHub 儲存庫 `bubble-tea-whack`
3. 建置設定：
   - Framework preset：`None`
   - Build command：留空
   - Build output directory：`/`（或留空）
4. 按 **Save and Deploy**，完成後會得到 `https://<專案名>.pages.dev`

之後每次 `git push` 到 `main`，Cloudflare 會自動重新部署。

## 授權
MIT
