# RT-Thread 近期任务社区工作总览

## 【申请中】【JOB201901】 at_device 软件包，适配更多模组

目前 at_device 软件包（ https://github.com/RT-Thread-packages/at_device ）是所有软件包中用的最多的一个，已经支持了近10种不同类似的模组

但还是有些常用的模组没有被适配进来，比如：air202, m6315 等等，大家可以选择自己熟悉的还未适配模组，进行适配

[点击这里](https://www.rt-thread.org/qa/forum.php?mod=viewthread&tid=7660) 查看模组适配的一些技术要求

## 【申请中】【JOB201902】ppp_device 软件包，适配更多模组

ppp_device 软件包（ https://github.com/RT-Thread-packages/ppp_device ）是最近新出的软件包，可以让网络协议栈跑在 MCU 这边，使用起来比 at_device 更加灵活，但也会略占更多资源

目前由于软件包刚发布，适配的模组还不多，可选适配的模组会比较多

[点击这里](https://github.com/RT-Thread-packages/ppp_device/blob/master/docs/port.md) 查看适配文档


## 【申请中】【JOB201903】基于 RT-Thread MicroPython 开发环境，开发更多创意 demo

近期 RT-Thread 正式发布了 MicroPython IDE V1.0 版本（ https://marketplace.visualstudio.com/items?itemName=RT-Thread.rt-thread-micropython ），该款 IDE 基于 VScode，与开发板连接后，可以直接在 VScode 上，对开发板进行 MicroPython 的开发。

对于 RT-Thread 定制的 STM32L475 潘多拉 IoT Board 及 W601 IoT Board ，该 MicroPython IDE 有专门的固件及示例与之对应，详见：https://github.com/RT-Thread/mpy-snippets/tree/master/examples/03.board

本次活动要求的 demo，必须基于 STM32L475 潘多拉 IoT Board 及 W601 IoT Board （PS：近期 W601 开发板还有赠送的活动），使用 Python 语言，控制开发板上硬件，比如：LCD，WiFi，按键，RGB

demo 实现功能范围没有要求，可以参考现在已有的实时天气的 demo ：

- 显示效果位于：插件介绍的 `Weather Show Demo 在开发板上的运行效果` 章节
- 源代码位于：https://github.com/RT-Thread/mpy-snippets/tree/master/demo/weather_show


## 【申请中】【JOB201904】基于 RT-Thread MicroPython 开发环境，开发更多驱动库或软件库

目前 RT-Thread MicroPython 开发环境支持的库还比较少，详见： https://github.com/RT-Thread/mpy-snippets/tree/master/library ，这些库类似于 RT-Thread 的软件包，为 Python 提供可重用软件的支持

希望开发者能使用 python 封装更多的驱动库（比如：数码管、LCD12864、DS18B20）及软件库（比如：xml解析、CoAP 等）

## 【申请中】【JOB201905】让 qemu 把 stm32 也模拟出来

目前的 qemu BSP 只要支持是的 A9 处理器，对于我们最常见的 STM32 芯片并为支持。

可以参考 GNU MCU Eclipse 已经支持了挺多 STM32 的 qemu ，可以参考 https://gnu-mcu-eclipse.github.io/qemu/

目 qemu 已经可以支持M4浮点了，所以希望我们能支持一款 M3/M4 的 qemu stm32 开发板，作为 BSP

以后开发调试，可以直接在 qemu 上完成。希望实现 stm32 qemu 模拟：uart，pin，文件系统等功能

## 【申请中】【JOB201906】传感器驱动软件包开发

当前 RT-Thread 已经支持了各种类型的传感器，( https://www.rt-thread.org/document/site/programming-manual/device/sensor/sensor_list/ )，对于上述列表中不支持的传感器，可以根据下述指南进行开发，做成软件包

[点击这里](https://www.rt-thread.org/document/site/development-guide/sensor/sensor_driver_development/) 查看传感器软件包开发指南

## 【申请中】【JOB201907】STM32 驱动开发

当前 RT-Thread 已经支持了很多 stm32 BSP， (https://github.com/RT-Thread/rt-thread/tree/master/bsp/stm32), 但是大部分 BSP 下仅支持了基本驱动，如 串口、GPIO，可以参考已经支持驱动较完善的 BSP，(https://github.com/RT-Thread/rt-thread/tree/master/bsp/stm32/stm32f429-atk-apollo), 来支持更多的外设驱动

## 【申请中】【JOB201908】imxRT 驱动开发

当前 RT-Thread 的 imxRT BSP 已经开发完成了很多外设驱动，(https://github.com/RT-Thread/rt-thread/tree/master/bsp/imxrt/libraries/drivers)， 还需要开发 SDIO，USB Device, Host 驱动

## 【申请中】【JOB201909】基于 RT-Robot 的智能车开发

基于 RT-Robot 软件包开发智能车，(https://github.com/RT-Thread-packages/rt-robot), 智能车实现功能范围没有要求


