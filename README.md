# ZMK board definition for pinkeybd

This repository contains the ZMK board definition and default keymap for the pinkeybd keyboard.

The default keymap is in `config/pinkeybd.keymap`. GitHub Actions builds the firmware automatically after a push to `main`; the resulting UF2 files are available from the workflow artifacts.

For local development, install the Zephyr SDK and `west`, then run:

```bash
west init -l . --mf config/west-workspace.yml
west update --narrow
west zmk-build
```
