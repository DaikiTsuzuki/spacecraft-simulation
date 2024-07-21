# spacecraft-simulation

## セットアップ
```
git clone https://github.com/DaikiTsuzuki/spacecraft-simulation.git
cd spacecraft-simulation
mkdir FlightSW 
cd FlightSW
git submodule add https://github.com/DaikiTsuzuki/c2a-aobc-hogesat.git
cd c2a-aobc-hogesat
git submodule init
git submodule update
cd ../..
git submodule add https://github.com/DaikiTsuzuki/s2e-aobc-hogesat.git
cd s2e-aobc-hogesat
git submodule init
git submodule update
```

## 使い方
基本的な使い方は[s2e-documents](https://github.com/ut-issl/s2e-documents)や[マニュアル資料](https://drive.google.com/drive/folders/1ulHbUkxzGktDtfjbGyPw3tFa1UGFzALS)を参照。

以下のファイルなどをシミュレーションする衛星に合うように修正する。
- s2e-aobc-hogesat/data/initialize_files/satellite_structure.ini
- c2a-aobc-hogesat/src/src_user/Settings/SatelliteParameters/Sample/structure_parameters.c

制御モードごとのサンプルは以下。

