# Flashing Meshtastic on Heltec V1 and Wio WM1110A

### Method:
Using Gitpod to compile compatible older versions.

### Compilation Commands:

**Heltec V1 and Wio WM1110A**:
Flash from binaries retrieved on Gitpod
```bash
pio run -e heltec-v1
pio run -e wio-tracker
python3 -m esptool --port /dev/ttyUSB1 --chip esp32 write_flash 0x0 firmware.factory.bin
```

# Issues Encountered with STM32 Boards

## Affected Boards

- Wyres V2  
- Seeed LoRa-E5 

We also have other boards such as **Wyres V2** and **LoRa-E5** that we would like to flash. These boards are based on **STM32** and are not directly compatible with **Meshtastic**.
Meshtastic is designed for **FreeRTOS**, while our boards use **RIOT-OS**.

To make them compatible, it would be necessary to:

- Take an existing Meshtastic firmware  
- Adapt it to work on STM32 boards running **RIOT-OS**  
- Develop a **compatibility API** between the **RadioLib** modules used by Meshtastic and the RIOT-OS environment  
- Flash them using a **Nucleo F334R8** board via ST-Link on an IDE such as **ArduinoIDE** or **STM32CubeProgrammer**.

This task, which we initially thought would be quickly achievable, turned out to be much more complex than expected. Not having anticipated this difficulty, we chose to focus on radio tests, which we considered a priority at this stage of the project.

In the end, the Meshtastic/STM32/RIOT-OS compatibility could not be finalized within the allotted time.