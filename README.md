# Dactyl-Manuform-6x6
Layout and files changed for the Dactyl Manuform 6x6 keyboard 

Download qmk_firmware_master from https://github.com/qmk/qmk_firmware

Within qmk_firmware/keyboards/dactyl-manuform do the following;
  1) Replace your dactyl-manuform.h with this one, it contains the basic layout for 6x6.
  2) Create a 6x6-default folder in the keymaps folder, and add config.h and keymap.c to the folder.
  3) Edit the MATRIX_ROW_PINS in config.h to add another pin. I added the pin D2. So the #define is now "#define MATRIX_ROW_PINS { D2, D4, C6, D7, E6, B4, B5 }"
  
The method for flashing this is exactly like flashing the 5x6 and other files.

"make 6x6-default" to just compile the firmware
"make 6x6-default-avrdude" to compile then flash

