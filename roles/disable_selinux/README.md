# disable_selinux

このロールはSELinuxの無効化を行います。

## 処理フロー

1. SELinuxの状態を取得し、表示

    **Disabled**ではない場合のみ以下タスクを実施

2. SELinuxの無効化とOS再起動(RHEL8以上で実施)

    RHEL7以下はSELinuxの無効化手順が異なるため実施しない

3. SELinuxの状態を取得し、表示
4. SELinuxのポリシー状態判定

    Disabledではない場合、異常終了とする

## 変数

なし

## 注意事項

なし
