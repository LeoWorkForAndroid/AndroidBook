## Android系统源码目录结构详解

### android平台四层架构对应源代码中的目录：

- 第一层：应用程序层(applications)对应根目录下packages/apps

- 第二层：应用程序框架层(application framework)对应根目录下的frameworks

- 第三层：运行库层包括运行库(libraries)和android运行时环境(android runtime)

      android运行时环境：

             Core Libraries 对应根目录下的libcore

             Dalvik Virtual Machine 对应根目录下的dalvik

   运行库libraries :

          libc对应根目录下的bionic

          其他的.......?

- 第四层：Linux内核层对应根目录下的kernel

三、四层中间还有个硬件抽象层(HAL)对应根目录下的hardware

## 详细目录结构如下：

#### 根目录
```

|-- Makefile
|
|-- bionic               （bionic C库）
|
|-- bootable             （启动引导相关代码）
|
|-- build                （存放系统编译规则及generic等基础开发包配置）
|
|-- cts                  （Android兼容性测试套件标准）
|
|-- dalvik               （dalvik JAVA虚拟机）
|
|-- development          （应用程序开发相关）
|
|-- external             （android使用的一些开源的模组）
|
|-- frameworks           （核心框架——java及C++语言）
|
|-- hardware             （部分厂家开源的硬解适配层HAL代码）
|
|-- out                  （编译完成后的代码输出与此目录）
|
|-- packages             （应用程序包）
|
|-- prebuilt             （x86和arm架构下预编译的一些资源）
|
|-- sdk                  （sdk及模拟器）
|
|-- system               （底层文件系统库、应用及组件——C语言）
|
|-- vendor               （厂商定制代码）

```

#### bionic 目录
```
|-- libc             （C库）
|   |-- arch-arm        （ARM架构，包含系统调用汇编实现）
|   |-- arch-x86        （x86架构，包含系统调用汇编实现）
|   |-- bionic                （由C实现的功能，架构无关）
|   |-- docs                （文档）
|   |-- include                （头文件）
|   |-- inet                （？inet相关，具体作用不明）
|   |-- kernel                （Linux内核中的一些头文件）
|   |-- netbsd                （？nesbsd系统相关，具体作用不明）
|   |-- private                （？一些私有的头文件）
|   |-- stdio                （stdio实现）
|   |-- stdlib                （stdlib实现）
|   |-- string                （string函数实现）
|   |-- tools                （几个工具）
|   |-- tzcode                （时区相关代码）
|   |-- unistd                （unistd实现）
|   `-- zoneinfo        （时区信息）
|-- libdl          （libdl实现，dl是动态链接，提供访问动态链接库的功能）
|-- libm           （libm数学库的实现，）
|   |-- alpha                （apaha架构）
|   |-- amd64                （amd64架构）
|   |-- arm                （arm架构）
|   |-- bsdsrc                （？bsd的源码）
|   |-- i386                （i386架构）
|   |-- i387                （i387架构？）
|   |-- ia64                （ia64架构）
|   |-- include                （头文件）
|   |-- man                （数学函数，后缀名为.3，一些为freeBSD的库文件）
|   |-- powerpc        （powerpc架构）
|   |-- sparc64                （sparc64架构）
|   `-- src                （源代码）
|-- libstdc++        （libstdc++ C++实现库）
|   |-- include                （头文件）
|   `-- src                （源码）
|-- libthread_db        （多线程程序的调试器库）
|   `-- include                （头文件）
`-- linker                        （动态链接器）
`-- arch                （支持arm和x86两种架构）

```

#### bootable  目录
```


```





#### build 目录
```


```

#### cts 目录
```


```

#### dalvik 目录
```


```



#### development 目录
```


```

#### external 目录
```


```

#### frameworks 目录
```


```

#### hardware 目录
```


```

#### out 目录
```


```

#### packages 目录
```


```

#### out 目录
```


```

#### prebuilt 目录

```

```

#### sdk 目录
```


```

#### system 目录
```


```

#### vendor 目录
```


```



