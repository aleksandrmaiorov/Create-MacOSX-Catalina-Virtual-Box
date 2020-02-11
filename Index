# How to Install macOS 10.15 Catalina on VirtualBox

#### Download macOS 10.15 Catalina and convert to ISO Image

##### Step 1
Download Catalina Final from the Mac App Store

[Download Catalina](https://apps.apple.com/us/app/macos-catalina/id1466841314?mt=12 "Download Catalina")
#### Step 2
##### Create macOS Catalina ISO File

Create a Catalina Virtual Disk Image
```bash
hdiutil create -o /tmp/Catalina -size 8500m -volname Catalina -layout SPUD -fs HFS+J
```
Mount this Image to macOS
```bash
hdiutil attach /tmp/Catalina.dmg -noverify -mountpoint /Volumes/Catalina
```
Use macOS Createinstallmedia Tool to create a Installer Image
```bash
sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/Catalina --nointeraction
```
Unmount Volume Catalina
```bash
hdiutil detach /volumes/Install\ macOS\ Catalina
```
Convert the Catalina.dmg to a Catalina.iso for Virtual Machine
```bash
hdiutil convert /tmp/Catalina.dmg -format UDTO -o ~/Desktop/Catalina.cdr
```
Move and Rename Catalina Image to Desktop
```bash
mv ~/Desktop/Catalina.cdr ~/Desktop/Catalina.iso
```

#### Step 3
##### Next install VirtualBox and then install the Extension Pack

[Download VirtualBox](https://techsviewer.com/go/virtualbox/ "Download VirtualBox")

#### Step 4

##### Create a New Virtual Machine


