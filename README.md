# payload.bin repack tool

Using delta_generator to repack `payload.bin`.

### Requirements

- A compatible Linux system (x86_64/aarch64)
- git
- openjdk-jre
- python
- python-protobuf 
- zip
- unzip
- openssl
- openssl-tool

### Linux X86-64 (Ubuntu)
```bash
sudo apt-get install git openssl openjdk-17-jre-headless python-protobuf python unzip zip
```

### Termux
```bash
pkg install git openssl-tool zip unzip python openjdk-17
```

## Installation
```bash
git clone https://github.com/snowwolf725/Payload_Repack_Tool.git
```

## Usage

### repack `payload.bin`

```bash
cd Payload_Repack_Tool
#copy *.img into IMAGES folder
#cp -a *.img IMAGES
./repackPayload.sh
```

### repack `payload.bin` with dynamic partition info

```bash
cd Payload_Repack_Tool
#copy *.img into IMAGES folder
#cp -a *.img IMAGES
#modify META/dynamic_partitions_info.txt
#vi META/dynamic_partitions_info.txt
./repackPayload_withDpart.sh
```

### repack `OTA.zip`

```bash
cd Payload_Repack_Tool
#copy *.img into IMAGES folder
#cp -a *.img IMAGES
#modify META/*.txt SYSTEM/build.prop
#vi META/*.txt SYSTEM/build.prop
./repackZip.sh
```

## Demo
【Android payload.bin 打包-哔哩哔哩】  https://www.bilibili.com/video/av113170408607840?p=1&unique_k=2333