# docker-ace-ja
日本語化した[Ace](https://daisy.github.io/ace/)をDockerイメージ化しました。
以下の方法で日本語のEPUBアクセシビリティレポートをコマンドラインで生成できます。

## clone Docker image
このリポジトリをcloneします。

```
> clone git@github.com:shunito/docker-ace-ja.git
```

## Build
以下のコマンドでdockerイメージをビルドします。

```
> cd docker-ace-ja
> docker-compose up -d
```

## Run (login docker image)
以下のコマンドでDocker imageにログインします。
```
> docker-compose exec ace bash
```

## Check
dataディレクトリにEPUBをコピーするとDocker image内で以下のコマンドでレポートが生成できます。

```
> ace -l ja -o ./report epubFileName.epub
```

- その他の使い方は[Ace Documents](https://daisy.github.io/ace/)を参照。
