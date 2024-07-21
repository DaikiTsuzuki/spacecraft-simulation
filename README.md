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

制御モードごとのサンプルは以下。
- https://github.com/DaikiTsuzuki/spacecraft-simulation/tree/BDOT
- https://github.com/DaikiTsuzuki/spacecraft-simulation/tree/ROUGH_SUN_POINTING
- https://github.com/DaikiTsuzuki/spacecraft-simulation/tree/ROUGH_THREE＿AXIS
- https://github.com/DaikiTsuzuki/spacecraft-simulation/tree/ROUGH_THREE_AXIS＿RW
- https://github.com/DaikiTsuzuki/spacecraft-simulation/tree/FINE_THREE_AXIS

