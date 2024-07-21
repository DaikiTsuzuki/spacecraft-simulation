# BDOT制御シミュレーションのやりかた

## セットアップ
mainブランチのセットアップを実施した後、以下のようにブランチを切り替える。
```
cd spacecraft-simulation
git branch BDOT
cd s2e-aobc-hogesat
git branch BDOT
```

## 使い方
1. 以下のファイルなどをシミュレーションする衛星に合うように修正する。
   - s2e-aobc-hogesat/data/initialize_files/satellite_structure.ini
   - c2a-aobc-hogesat/src/src_user/Settings/SatelliteParameters/Sample/structure_parameters.c
1. BDOT
   - s2e-aobc-hogesat/data/initialize_files/components/wings_command_sender_to_c2a/example.ops
   - s2e-aobc-hogesat/data/initialize_files/components/wings_command_sender_to_c2a/wings_command_sender_to_c2a.ini

## 結果の例
シミュレーションの初期状態などはコードを参照のこと。

シミュレーションを実行結果を以下に示す。
角速度が下がっていることを確認できる。
![result(angular_velocity)](result(angular_velocity).png)