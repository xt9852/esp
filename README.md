# ESP8266

------

## 软硬件
> * 使用的nodeMCU模块进行开发，些模块使用的是esp12f芯片
> * 使用RTOS的[SDK](https://github.com/espressif/ESP8266_RTOS_SDK)进行开发

## 开发步骤
> * [下载](https://github.com/espressif/ESP8266_RTOS_SDK)交叉编译工具
> * [下载](https://github.com/espressif/ESP8266_RTOS_SDK)SDK
> * 设置参数: export IDF_PATH=~/esp/ESP8266_RTOS_SDK
> * 进入目录: cd ~/esp/ESP8266_RTOS_SDK/examples/get-started/hello_world
> * 执行命令1: make menuconfig
> * 执行命令2: make
> * 执行命令3: make flash
> * 执行命令4: make monitor

## 实例
> * 复制SDK目录examples\storage进行修改
> * partitions_example.csv做为分区使用的，如果不使用文件系统可以删除，如果使用需要执行make menuconfig中配置存储项目中将配置文件名添加上
> * 修改Make,CMakeLists,main\CMakeLists这几个文件中的项目名称
> * 修改main\spiffs_example_main.c文件同项目名
> * 进行编译，下载程序到模块，运行程序
