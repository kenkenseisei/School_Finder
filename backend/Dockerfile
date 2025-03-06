# Maven付きのJDKイメージを使用
FROM maven:3.9-eclipse-temurin-17

# 作業ディレクトリを作成
WORKDIR /app

# ソースコードをコピー
COPY . .

# Mavenでビルド
RUN mvn clean package

# ポートを公開
EXPOSE 8080

# 実行
CMD ["java", "-jar", "target/backend-0.0.1-SNAPSHOT.jar"]
