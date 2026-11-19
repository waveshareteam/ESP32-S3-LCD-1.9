# Factory firmware

Flash the merged BIN at **0x0** on ESP32-S3-LCD-1.9 (ESP32-S3, 16MB Flash).

| Firmware | Date | Description | Offset |
| --- | --- | --- | --- |
| [ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin](ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin) | 2025-04-08 | Factory firmware | `0x0` |

```shell
python -m esptool --chip esp32s3 erase_flash
python -m esptool --chip esp32s3 write_flash 0x0 ESP32-S3-LCD-1.9_FactoryOnly_20250408.bin
```

Disconnect other boards and select the device port with `--port` if needed.
