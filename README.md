# Yubico Authenticator Flatpak

Unofficial [Flathub package](https://flathub.org/apps/details/com.yubico.yubioath) of [Yubico Authenticator](https://developers.yubico.com/yubioath-desktop/) to read TOTP codes (6 digits 2FA) from YubiKey.

## Install Instructions:
> [!IMPORTANT]
   You must install **PCSC daemon** to use this app.
>
> Ubuntu: `sudo apt install pcscd`
> 
> Fedora: `sudo dnf install pcsc-lite`
>
> Then run `pcscd -v` to check which version of pcsc daemon is installed.

**For distros that use pcsc version 2.3.0 and above, use the beta version of this flatpak. DON'T report pcsc issues to Yubico.**

## Install for systems with pcsc daemon >= 2.3.0 (Fedora 41)
Open a terminal and run:
```
flatpak uninstall com.yubico.yubioath
flatpak remote-add --user --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
flatpak install flathub-beta com.yubico.yubioath
```

## Systems with pcscd version <= 2.0.3

Install from the main Flathub repo, Software center, or run:

   ```sh
   flatpak install flathub com.yubico.yubioath
   ```
