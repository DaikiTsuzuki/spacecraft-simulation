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