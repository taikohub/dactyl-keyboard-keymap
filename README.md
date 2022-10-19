# Taikohub Dactyl Manuform Keyboard Keymap Examples
- These folders contain example keymaps for the [taikohub dactyl manuform keyboard](https://taikohub.com).
- This is part of the [Customizing Keyboard Layout for Linux with QMK](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk) section for the taikohub dactyl keyboard documentation, which can be found at [docs.taikohub.com](https://docs.taikohub.com).

## Instructions
1. You must have already downloaded the QMK CLI tool. If you haven't done this already, see [Customizing Keyboard Layout for Linux with QMK](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk).

2. If you have reached section [4.5 📝Keymap  - Editing keymap.c](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk#4.5-keymap-editing-keymap.c), continue along these steps. Start by cloning this repo.
```
git clone https://github.com/taikohub/dactyl-keyboard-keymap.git
```

3.a. Copy the relevant folder into qmk's configuration files. The `five_key` folder is for the five keyed thumb cluster keyboard (size medium). The `six_key` folder is for the six keyed thumb cluster keyboard (size large). If you are following the documentation exactly from the website and you use a size medium keyboard, just replace the `keymap.c` file in your keymap with the one in `/five_key/keymap.c` in this repo.
```
cp five_key/keymap.c -r ~/qmk_firmware/keyboards/handwired/dactyl_manuform/5x6/keymaps/taiko/keymap.c
```
Then follow the rest of the documentation, continuing with section [4.6 🖥️Keyboard - Flashing the Firmware](https://docs.taikohub.com/customizing-keyboard-layout-for-linux-with-qmk#4.6-keyboard-flashing-the-firmware). 


3.b. Alternatively: If you didn't run `qmk new-keymap -kb handwired/dactyl_manuform/5x6`, you can just copy the entire folder.
```
cp five_key -r ~/qmk_firmware/keyboards/handwired/dactyl_manuform/5x6/keymaps/
```
Please make sure you enter the above with the `/` at the end.
You would then flash it using the command below instead of `qmk flash -kb handwired/dactyl_manuform/5x6 -km taiko`.
```
qmk flash -kb handwired/dactyl_manuform/5x6 -km five_key
```
