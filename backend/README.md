# survey_delve

go mod init survey_delve

https://gin-gonic.com/ja/docs/quickstart/　

go get -u github.com/gin-gonic/gin

main.goにサンプルコードをコピペ

go run main.go　でサーバー起動

curl http://localhost:8080/ping でアクセステスト


### air
https://github.com/air-verse/air

go install github.com/air-verse/air@latest でairをインストール

air init で設定ファイルを作成

~/.zshrcファイルにGOPATHとGOBINの設定を追加します。
echo 'export GOPATH=$HOME/go' >> ~/.zshrc
echo 'export GOBIN=$GOPATH/bin' >> ~/.zshrc
echo 'export PATH=$PATH:$GOBIN' >> ~/.zshrc

~/.zshrcファイルを再読み込みします。
source ~/.zshrc

dlvとairを再インストールします。
go install github.com/go-delve/delve/cmd/dlv@latest
go install github.com/air-verse/air@latest

インストールが成功したか確認します。
dlv version
air -v

```
