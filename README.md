This project targets [ESP32-DevKitC V4 ](https://docs.espressif.com/projects/esp-idf/en/latest/hw-reference/get-started-devkitc.html)

[schematic](https://dl.espressif.com/dl/schematics/esp32_devkitc_v4-sch.pdf)

Covers the following modules,
- ESP32-WROOM-32
- ESP32-WROOM-32D
- ESP32-WROOM-32U
- ESP32-SOLO-1
- ESP32-WROVER
- ESP32-WROVER-B
- ESP32-WROVER-I
- ESP32-WROVER-B (IPEX)

## Setup
mac instructions, windows will be similar.

### prereqs
1. `pip install --user virtualenv`
2. create a virtual environment
    - `virtualenv venv`
    - `source venv/bin/activate`
3. `pip install pyserial`
4. `brew install cmake ninja ccache`
5. `git submodule update --init --recursive`

### tools
1. `cd` to your normal repo clone directory, you will be cloning a new repo
2. `git clone https://github.com/espressif/esp-idf.git --recursive`
3. `cd esp-idf`
4. `./install.sh` (creates tools in home dir *~\.espressif* & environment variable *IDF_TOOLS_PATH*)
5. `. export.sh`


### start project
1. `idf.py menuconfig`