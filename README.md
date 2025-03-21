
This model can be built by ROSS by sym-linking it into the ROSS/models directory and building with `-DROSS_BUILD_MODELS=ON`

``` shell
git clone https://github.com/ROSS-org/ROSS
git clone https://github.com/ROSS-org/template-model
cd ROSS/models
ln -s ../../template-model ./
(on windows, the command is mklink /D model-link ../path-to-model)
(^^ must open terminal as admin)
cd ../
mkdir build
cmake ../ -DROSS_BUILD_MODELS=ON
make
```
