# docker run

> 新しいDockerコンテナでコマンドを実行します。
> もっと詳しく: <https://docs.docker.com/reference/cli/docker/container/run/>。

- タグ付けイメージから作成した新しいコンテナでコマンドを実行する:

`docker run {{イメージ:タグ}} {{コマンド}}`

- 新しいコンテナでコマンドをバックグランド実行し、そのIDを表示する:

`docker run {{[-d|--detach]}} {{イメージ}} {{コマンド}}`

- インタラクティブモードと疑似端末の割り当てを行って、使い捨てコンテナでコマンドを実行する:

`docker run --rm {{[-it|--interactive --tty]}} {{イメージ}} {{コマンド}}`

- 渡された環境変数を使って新しいコンテナでコマンドを実行する:

`docker run {{[-e|--env]}} '{{環境変数名}}={{値}}' {{[-e|--env]}} {{環境変数名}} {{イメージ}} {{コマンド}}`

- バインドマウントを持つ新しいコンテナでコマンドを実行する:

`docker run {{[-v|--volume]}} {{ホストへのパス}}:{{コンテナへのパス}} {{イメージ}} {{コマンド}}`

- 公開ポートを持った新しいコンテナでコマンドを実行する:

`docker run {{[-p|--publish]}} {{ホスト側のポート}}:{{コンテナ側のポート}} {{イメージ}} {{コマンド}}`

- イメージのエントリーポイントを上書きして新しいコンテナでコマンドを実行する:

`docker run --entrypoint {{コマンド}} {{イメージ}}`

- 新しいコンテナをネットワークに繋ぎ、そのコンテナでコマンドを実行する:

`docker run --network {{ネットワーク}} {{イメージ}}`
