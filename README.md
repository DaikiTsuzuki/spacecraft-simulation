# 【WIP】粗太陽捕捉シミュレーションのやりかた

## セットアップ
mainブランチのセットアップを実施した後、以下のようにブランチを切り替える。
```
cd spacecraft-simulation
git branch ROUGH_SUN_POINTING
cd s2e-aobc-hogesat
git branch ROUGH_SUN_POINTING
```

## 使い方
1. 以下のファイルなどをシミュレーションする衛星に合うように修正する。
   - s2e-aobc-hogesat/data/initialize_files/satellite_structure.ini
   - c2a-aobc-hogesat/src/src_user/Settings/SatelliteParameters/Sample/structure_parameters.c
1. ROUGH_SUN_POINTINGの設定をする
   - s2e-aobc-hogesat/data/initialize_files/components/wings_command_sender_to_c2a/example.ops
   - s2e-aobc-hogesat/data/initialize_files/components/wings_command_sender_to_c2a/wings_command_sender_to_c2a.ini

## 結果の例
シミュレーションの初期状態などはコードを参照のこと。

シミュレーションを実行結果を以下に示す。
シミュレーションを実行結果を以下に示す。 太陽捕捉できていない…（要修正）
![result(angular_velocity)](result(angular_velocity).png)
![result(angular_velocity)](result(quaternion_i2b).png)
![result(sun_position)](result(sun_position).png)