# BIOSUtilities
Various BIOS Utilities for Modding/Research

[BIOS Utilities News Feed](https://twitter.com/platomaniac)

[![BIOS Utilities Donation](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=DJDZD3PRGCSCL)

![](https://i.imgur.com/ci3H4Y3.png)

## **Dell HDR Module Extractor**

#### **Description**

Parses modern icon-less Dell BIOS HDR executables and extracts their SPI/BIOS modules. After extraction, the HDR image is automatically unpacked into individual SPI/BIOS modules via [LongSoft's PFSExtractor-RS](https://github.com/LongSoft/PFSExtractor-RS) tool.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Dell HDR executables.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script or its built/frozen/compiled binary, you need to have the following 3rd party tool at the same directory:

* [PFSExtractor-RS](https://github.com/LongSoft/PFSExtractor-RS) (i.e. PFSExtractor.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Dell_HDR_Extract.py

At dist folder you should find the final utility executable

## **AMI BIOS Guard Extractor**

#### **Description**

Parses AMI BIOS Guard (a.k.a. PFAT) images and extracts a proper SPI/BIOS image.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing AMI PFAT images.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the utility, you do not need any 3rd party tool.

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile AMI_PFAT_Extract.py

At dist folder you should find the final utility executable

## **Apple EFI Sucatalog Link Grabber**

#### **Description**

Parses Apple Software Update CatalogURL .sucatalog files and saves all EFI firmware package links into a text file. It removes any xml formatting, ignores false positives, removes duplicate links and sorts them in alphabetical order for easy comparison afterwards.

#### **Usage**

You can either Drag & Drop or let it automatically parse any .sucatalog files within its working directory.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the utility, you do not need any 3rd party tool.

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Apple_EFI_Links.py

At dist folder you should find the final utility executable

## **Apple EFI File Renamer**

#### **Description**

Parses Apple EFI files and renames them based on Intel's official $IBIOSI$ tag as follows: Model_Version_Build_Year_Month_Day_Hour_Minute_Checksum. The checksum is calculated and added by the utility in order to differentiate any EFI files with the same $IBIOSI$ tag. In rare cases in which the $IBIOSI$ tag is compressed, the utility automatically first uses [LongSoft's UEFIFind and UEFIExtract](https://github.com/LongSoft/UEFITool) tools.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Apple EFI firmware.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script or its built/frozen/compiled binary, you need to have the following 3rd party tools at the same directory:

* [UEFIFind](https://github.com/LongSoft/UEFITool) (i.e. UEFIFind.exe)
* [UEFIExtract](https://github.com/LongSoft/UEFITool) (i.e. UEFIExtract.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Apple_EFI_Rename.py

At dist folder you should find the final utility executable

## **Apple EFI IM4P Splitter**

#### **Description**

Parses Apple multiple EFI firmware .im4p files and splits all detected EFI firmware into separate SPI/BIOS images.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Apple EFI IM4P firmware.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the utility, you do not need any 3rd party tool.

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Apple_EFI_Split.py

At dist folder you should find the final utility executable

## **Panasonic BIOS Update Extractor**

![](https://i.imgur.com/uZAoMGR.png)
<sub><sup>*Icon owned by Panasonic*</sup></sub>

#### **Description**

Parses Panasonic BIOS Update executables and extracts their SPI/BIOS image. The utility automatically uses [Rustam Abdullaev's unpack_lznt1](https://github.com/rustyx/unpack_lznt1) tool in order to decompress the initially Microsoft LZNT1 compressed resource data.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Panasonic BIOS Update executables.

#### **Download**

An already built/frozen/compiled Windows binary is provided by me. Thus, **you don't need to manually build/freeze/compile it**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script, you need to have the following 3rd party Python modules installed:

* [PEfile](https://pypi.python.org/pypi/pefile/)

> pip3 install pefile

To run the python script or its built/frozen/compiled binary, you need to additionally have the following 3rd party tool at the same directory:

* [unpack_lznt1](https://github.com/rustyx/unpack_lznt1) (i.e. unpack_lznt1.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at Windows, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Use pip to install PEfile:

> pip3 install pefile

4. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Panasonic_BIOS_Extract.py

At dist folder you should find the final utility executable

## **VAIO Packaging Manager Extractor**

![](https://i.imgur.com/rg4xrxJ.png)
<sub><sup>*Icon owned by VAIO*</sup></sub>

#### **Description**

Parses VAIO Packaging Manager executables and extracts their contents. If direct extraction fails, it unlocks the executable in order to run at all systems and allow the user to choose the extraction location. The utility automatically uses [Igor Pavlov's 7-Zip](https://www.7-zip.org/) tool in order to decompress the initially obfuscated Microsoft CAB compressed contents.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing VAIO Packaging Manager executables.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script or its built/frozen/compiled binary, you need to have the following 3rd party tool at the same directory:

* [7-Zip Console](https://www.7-zip.org/) (i.e. 7z.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile VAIO_Package_Extract.py

At dist folder you should find the final utility executable

## **Fujitsu SFX Packager Extractor**

![](https://i.imgur.com/NlZGBsy.png)
<sub><sup>*Icon owned by FUJITSU*</sup></sub>

#### **Description**

Parses Fujitsu SFX Packager executables and extracts their contents. The utility automatically uses [Igor Pavlov's 7-Zip](https://www.7-zip.org/) tool in order to decompress the initially obfuscated Microsoft CAB compressed contents.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Fujitsu SFX Packager executables.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script or its built/frozen/compiled binary, you need to have the following 3rd party tool at the same directory:

* [7-Zip Console](https://www.7-zip.org/) (i.e. 7z.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Fujitsu_Package_Extract.py

At dist folder you should find the final utility executable

## **Award BIOS Module Extractor**

#### **Description**

Parses Award BIOS images and extracts their modules. The utility automatically uses [Igor Pavlov's 7-Zip](https://www.7-zip.org/) tool in order to decompress the initially LZH compressed sub-modules.

#### **Usage**

You can either Drag & Drop or manually enter the full path of a folder containing Award BIOS firmware.

#### **Download**

An already built/frozen/compiled binary is provided by me for Windows only. Thus, **you don't need to manually build/freeze/compile it under Windows**. Instead, download the latest version from the [Releases](https://github.com/platomav/BIOSUtilities/releases) tab. To extract the already built/frozen/compiled archive, you need to use programs which support RAR5 compression. Note that you need to manually apply any prerequisites.

#### **Compatibility**

Should work at all Windows, Linux or macOS operating systems which have Python 3.6 support. Windows users who plan to use the already built/frozen/compiled binary must make sure that they have the latest Windows Updates installed which include all required "Universal C Runtime (CRT)" libraries.

#### **Prerequisites**

To run the python script or its built/frozen/compiled binary, you need to have the following 3rd party tool at the same directory:

* [7-Zip Console](https://www.7-zip.org/) (i.e. 7z.exe)

#### **Build/Freeze/Compile with PyInstaller**

PyInstaller can build/freeze/compile the utility at all three supported platforms, it is simple to run and gets updated often.

1. Make sure Python 3.6.0 or newer is installed:

> python --version

2. Use pip to install PyInstaller:

> pip3 install pyinstaller

3. Build/Freeze/Compile:

> pyinstaller --noupx --onefile Award_BIOS_Extract.py

At dist folder you should find the final utility executable