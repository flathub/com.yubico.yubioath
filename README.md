# Yubico Authenticator Flatpak

Unofficial [Flathub package](https://flathub.org/apps/details/com.yubico.yubioath) of [Yubico Authenticator](https://developers.yubico.com/yubioath-desktop/) to read TOTP codes (6 digits 2FA) from YubiKey.

You need to install **PCSC daemon** to use this app.

**NOTE: This (community) flatpak currently works only with distros that use version of pcsc-lite below 2.3.0. For distros that use version 2.3.0 and above use beta version of this flatpak. DON'T report this to Yubico.**

## Install

1. [Add Flathub](https://flatpak.org/setup/) to your system.
2. Install PCSC daemon.

   ```sh
   sudo dnf install pcsc-lite
   ```
3. Install Yubico Authenticator from Flathub:

   ```sh
   flatpak install flathub com.yubico.yubioath
   ```
