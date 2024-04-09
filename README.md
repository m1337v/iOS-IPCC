# iOS-IPCC
IPCC bundle files for different iOS Versions and devices. Update your carrier bundle (no jailbreak required)

# Usage
1. Search for your device e.g. iPhone 12 Pro Max.
2. Search for an iOS higher than your current iOS e.g. 14.8 when you have 14.3 installed.
- You can do this manually too if you prefer by downloading the respective ipsw file from [ipsw.me](http://ipsw.me). Extract it and mount the largest dmg file. Navigate to System>Library>Carrier Bundles>iPhone.
3. Search for your carrier and copy the bundle file to your Computer e.g. "TMobile_Germany.bundle".
4. Create a new folder named "Payload".
5. Copy the bundle file inside the "Payload" folder.
6. Zip the "Payload" folder and rename it as per your carrier bundle with an ipcc extension e.g. "TMobile_Germany.ipcc".
7. Enable .ipcc support in iTunes/Finder by opening Terminal (on Mac) or CMD (on Windows) and pasting the following command:
- macOS 10.14 and older
   ```
   defaults write com.apple.itunes carrier-testing -bool true
   ```
- macOS 10.15 and newer
  ```
  defaults write com.apple.AMPDevicesAgent carrier-testing -bool YES
  ```
- Windows
  ```
  "%ProgramFiles%\iTunes\iTunes.exe" /setPrefInt carrier-testing 1
  ```
8. Now use iTunes/Finder to update the .ipcc carrier bundle. While pressing Option (Mac) or Shift (Windows) in iTunes/Finder, click on update and select the .ipcc file.
9. Restart your iPhone.
