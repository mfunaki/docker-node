FROM cimg/base:stable

# ADD, COPY, RUNコマンドを実行するごとに、ビルドにレイヤーが追加されるため、
# 可能な限りコマンドをチェーンする
RUN sudo apt-get update && sudo apt-get install -y \
        git nodejs npm && \
    sudo rm -rf /var/lib/apt/lists/*
## 最後の行でイメージ内のAptキャッシュを削除し、イメージのサイズを抑える

CMD [ "/bin/bash" ]