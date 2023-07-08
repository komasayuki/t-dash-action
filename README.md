# GitHub Custom Action for T-Dash Testing

これはGitHub ActionsでT-Dashを使ったテストをするためのCustom Actionです。
T-DashのテストをGitHub Actionsに組み込むことを支援します。

## 前提条件
GitHub ActionsのRunner OSがwindowsであること。

## 使い方

以下のように使います。

`sync-path` はT-DASHでエクスポートしたsyncフォルダーのパスです。
`test-run-name`はT-DASHで作成したテストランの名前です。

```yml
- uses: komasayuki/t-dash-action-win@v1
    with:
        sync-path: test/t-dash/sync
        test-run-name: all
```

実際のプロジェクトでの利用例は、以下のプロジェクトを見てください。
http://github.com/komasayuki/t-dash-example

