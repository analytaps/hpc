High Perforamce Computing library

# Build HPC library

```
export RTE_SDK=${HPC_DIR}
export RTE_TARGET=x86_64-native-linuxapp-gcc

make install T=x86_64-native-linuxapp-gcc
```

# Build examples
```
cd example
cd helloworld
make
./build/helloword -c 1 -n 2
```
