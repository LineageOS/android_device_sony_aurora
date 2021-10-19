# Device Tree for Xperia XZ2 Premium (aurora)
The Xperia (codenamed _"aurora"_) is a smartphone from Sony Mobile.
It was released in 2018.

| Basic                   | Spec Sheet                                                                                                                                    |
| -----------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------- |
| CPU                     | Octa-core (4x2.7 GHz Kryo 385 Gold & 4x1.7 GHz Kryo 385 Silver)                                                                               |
| Chipset                 | Qualcomm SDM845 Snapdragon 845                                                                                                                |
| GPU                     | Adreno 630                                                                                                                                    |
| Memory                  | 6 GB RAM                                                                                                                                      |
| Shipped Android Version | 8.0                                                                                                                                           |
| Storage                 | 64 GB                                                                                                                                         |
| Battery                 | Non-removable Li-Ion 3540 mAh battery                                                                                                         |
| Display                 | Toppest LCD, 2160 x 3840 pixels, 16:9 ratio (~765 ppi density)                                                                                |
| Camera (Back)           | 19 MP (f/1.8, 25mm, 1/2.3", 1.22 µm), gyro EIS, predictive phase detection and laser AF, LED flash, 4K at 30fps, 1080p at 30, 60fps or 960fps |
|                         | 12 MP (f/1.6, 1/2.3", 1.55 µm), predictive phase detection                                                                                    |
| Camera (Front)          | 13 MP (f/2.0, 1/3.1"), gyro EIS, 1080p                                                                                                        |

Copyright 2018 - The LineageOS Project.

![Xperia XZ2 Premium](https://images-na.ssl-images-amazon.com/images/I/61G48YhuWmL._AC_SL1200_.jpg "Xperia XZ2 Premium")


## Temporary build instructions

```
# Compiling
$ m[ake|ka] bootimage systemimage

# Installing
$ fastboot --disable-verity --disable-verification flash vbmeta stock_vbmeta.img
$ fastboot flash boot boot.img
$ fastboot flash system system.img
$ fastboot -w reboot
```

