# Yubico Authenticator Flatpak

Unofficial [Flathub package](https://flathub.org/apps/details/com.yubico.yubioath) of [Yubico Authenticator](https://developers.yubico.com/yubioath-desktop/) to read TOTP codes (6 digits 2FA) from YubiKey.

You need to install **PCSC daemon** to use this app.


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
