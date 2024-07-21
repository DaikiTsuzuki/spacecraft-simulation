# 【WIP】精三軸制御制御シミュレーションのやりかた

## セットアップ
mainブランチのセットアップを実施した後、以下のようにブランチを切り替える。
```
cd spacecraft-simulation
git branch FINE_THREE_AXIS
cd s2e-aobc-hogesat
git branch FINE_THREE_AXIS
cd FlightSW/c2a-aobc-hogesat
git branch FINE_THREE_AXIS
```

## 使い方
1. 以下のファイルなどをシミュレーションする衛星に合うように修正する。
   - s2e-aobc-hogesat/data/initialize_files/satellite_structure.ini
   - c2a-aobc-hogesat/src/src_user/Settings/SatelliteParameters/Sample/structure_parameters.c
2. 精三軸制御制御のための設定をする。
   - FlightSW/c2a-aobc-hogesat/src/src_user/Settings/Modes/Transitions/sl_initial.c
   - FlightSW/c2a-aobc-hogesat/src/src_user/Settings/Modes/TaskLists/tl_initial.c

## 結果の例
シミュレーションの初期状態などはコードを参照のこと。

シミュレーションを実行結果を以下に示す。
収束していない…（要修正）
![result(angular_velocity)](result(angular_velocity).png)
![result(quaternion_i2b)](result(quaternion_i2b).png)