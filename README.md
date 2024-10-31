# SaintCon2024Badge-Sandbox
My sandbox for hacking the SaintCon2024 Badge

## Secret messages???

```
NKFSRBDKWALKBCYKDXPXRWUFXCYXEISDRWK
A9 ROA 1940
```

10/29/2024
- Worked through a number of ciphers, haven't cracked it yet.
- A9, 1940 -- Cruicer Mk I tank????
- ROA -- Return on assets?  ROA/1940 -- Russian Liberation Army?

```
Hey, Listen!
```

Shut up, Navi.

## ESP32-S3

- Technical manual: https://www.espressif.com/sites/default/files/documentation/esp32-s3_technical_reference_manual_en.pdf

- Dump flash:

```python
python esptool.py -b 115200 --port COM3 read_flash 0x000000 0x400000 flash_4M.bin
```

- Load flash:

```python
python esptool.py -b 115200 --port COM3 write_flash --flash_freq 80m 0x000000 flash_4M.bin
```