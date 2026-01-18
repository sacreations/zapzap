# ZapZap - Personal Fork

This is a personal fork of ZapZap for custom modifications and personal use.

**Original Repository:** [rafatosta/zapzap](https://github.com/rafatosta/zapzap)

## About ZapZap

ZapZap is an unofficial WhatsApp Desktop application for Linux, built with PyQt6 + PyQt6-WebEngine.

## Custom Modifications

This fork includes the following enhancements:

- **Native WhatsApp Context Menu**: Added option to use native WhatsApp context menu in WebView instead of Qt's default context menu
- **Arch Linux Packaging**: Added `PKGBUILD` for easy installation on Arch-based systems

## Installation (Arch Linux)

```bash
makepkg -si
```

## Requirements

- Python 3.9+
- PyQt6
- PyQt6-WebEngine
- dbus-python

## License

GPL-3.0 - See the [original repository](https://github.com/rafatosta/zapzap) for full license details.

## Credits

Original author: [Rafael Tosta](https://github.com/rafatosta)