# Taikohub Dactyl Manuform Keyboard Keymap Examples
- These files contain example keymaps for the [taikohub](https://taikohub.com) dactyl manuform keyboard.
- They follow the documentation seen here]([taikohub](https://taikohub.com).
- These are part of the [Customizing Keyboard Layout for Linux with QMK - Editing keymap.c](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk#4.5-keymap-editing-keymap.c) section at [docs.taikohub.com](https://docs.taikohub.com).

## How do I use this
1. You must have already downloaded the QMK CLI tool. If you haven't, see [Customizing Keyboard Layout for Linux with QMK](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk).

2. Clone the repo.
`git clone https://github.com/taikohub/dactyl-keyboard-keymap.git`

3. Copy the appropriate folder into qmk's configuration files. The `five_key` folder is for the five keyed thumb cluster keyboard (size medium). The `six_key` folder is for the six keyed thumb cluster keyboard (size large).
`cp five_key -r ~/qmk_firmware/keyboards/handwired/dactyl_manuform/5x6/keymaps/`

4. Follow the rest of the documentation, continuing with section [Flashing the Firmware](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk#4.6-keyboard-flashing-the-firmware).