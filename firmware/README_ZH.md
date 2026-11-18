# 出厂固件

适用于 ESP32-S3-LCD-1.9（ESP32-S3，16MB Flash），合并 BIN 从 **0x0** 烧录。

| 固件 | 日期 | 用途 | 烧录偏移 |
| --- | --- | --- | --- |
| [ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin](ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin) | 2025-04-08 | 出厂固件 | `0x0` |

```shell
python -m esptool --chip esp32s3 erase_flash
python -m esptool --chip esp32s3 write_flash 0x0 ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin
```

断开其他开发板；需要指定设备时使用 `--port` 参数。
