# konaste-resolution-changer

## なにこれ
解像度を変更するPowerShellと利用しているバッチファイルのまとめ

beatmanieaIIDX INFINITASの起動と合わせて変更するサンプル付き

該当のバッチをショートカットとしてデスクトップなどにおいて使用してください。

## 使い方

### 終了時用のバッチを作る
公開しているバッチは
- 1920*1080 120hz
- 3840*2160 144hz

に変更するバッチファイルが入っています。
それ以外の解像度やリフレッシュレートに変更したい場合は、以下の手順に沿って新規のバッチファイルを作成してください。

1. 同じフォルダで新規のテキストを作成
2. 以下の内容を記載し<名前>.batとして保存
```
powershell -NoProfile -ExecutionPolicy Unrestricted .\set-screen-size.ps1 <画面の横幅> <画面の立幅> <リフレッシュレート>
```

例) 2560x1440 240hzにしたい場合
```
powershell -NoProfile -ExecutionPolicy Unrestricted .\set-screen-size.ps1 2560 1440 240
```

### INFINITASを起動する場合
1. start_beatmaniaIIDX_INFINITAS.batを実行してください
2. 終了時には該当の解像度/リフレッシュレートに変更するバッチを実行してください