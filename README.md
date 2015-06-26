High Perforamce Computing library

# Build HPC library

```
export RTE_SDK=$PWD
export RTE_TARGET=x86_64-native-linuxapp-gcc

make install T=x86_64-native-linuxapp-gcc
```

# Configure Hugepage
To execute application, it needs hugepage setting.
Temporary setting is,
```
echo 1024 > /sys/kernel/mm/hugepages/hugepages-2048kB/nr_hugepages
mkdir /hugepage
mount -t hugetlbfs nodev /hugepage
```

# Build examples
```
cd example
cd helloworld
make
./build/helloword -c 1 -n 2
```
