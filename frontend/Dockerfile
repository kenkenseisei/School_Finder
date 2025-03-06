# Node.jsの公式イメージを使用
FROM node:18-alpine

# 作業ディレクトリを設定
WORKDIR /app

# package.jsonとpackage-lock.jsonをコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm install

# Reactアプリのソースをコピー
COPY . .

# ポート公開
EXPOSE 3000

# アプリの起動
CMD ["npm", "start"]
