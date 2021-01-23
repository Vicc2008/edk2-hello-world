# edk2-hello-world
hello-world firmware edk2 for uefi shell

## Dependencies

Ubuntu 18.04:

```
sudo apt update
sudo apt install build-essential uuid-dev iasl git nasm python3-distutils gcc-aarch64-linux-gnu abootimg figlet
```
Or
```
sudo apt install build-essential
sudo apt install build-essential
sudo apt install uuid-dev
sudo apt install iasl
sudo apt install git
sudo apt install nasm
sudo apt install python3-distutils
sudo apt install gcc-aarch64-linux-gnu
sudo apt install abootimg
sudo apt install figlet
```


## Building
1.Clone edk2 and edk2-platforms (Place three directories side by side.)

edk2:
```
commit:3a3713e62cfad00d78bb938b0d9fb1eedaeff314
```

edk2-platforms:
```
commit:cfdc7f907d545b14302295b819ea078bc36c6a40
```

```
mkdir workspaceedk2
cd workspaceedk2
git clone https://github.com/tianocore/edk2.git -o 3a3713e62cfad00d78bb938b0d9fb1eedaeff314 --recursive --depth=1
git clone https://github.com/tianocore/edk2-platforms.git -o cfdc7f907d545b14302295b819ea078bc36c6a40 --recursive --depth=1
```

2.Clone this project
```
git clone https://github.com/Vicc2008/edk2-hello-world.git
```

3.Build environment
```
cd edk2-hello-world
bash firstrun.sh
```

4.Build this project
```
bash build.sh
```
5.Debug and use
```
fastboot boot uefi.img
```
