# Node.js + Java入りのベースイメージを使う
FROM mcr.microsoft.com/devcontainers/java:11

# Vue.js 開発用に Node.js を追加
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash - && \
    apt-get install -y nodejs

# npmとvueのCLIをグローバルに入れる
RUN npm install -g @vue/cli

# Gitが入っていない場合は追加（このベースには入ってるはず）
# RUN apt-get install -y git