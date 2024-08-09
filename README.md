# moil_coffee

[![q51210_coffee](https://img.youtube.com/vi/it3XaNYqQ_c/0.jpg)](https://www.youtube.com/watch?v=it3XaNYqQ_c)   

Purpose : This repository is based on the Coffee exmaple project in Qt5.12.10.

We modify the code and some libraries, functions and parameters to make it run in Qt5.6.3

## 1. Prerequisites

Prepare a Renesas RZ/G2L board running a pre-build BSP image or yocto build image by using 'core-image-qt' . We will transfer and execute our code on it later.

Also install Qt5.6.3 and Qt Creator and setup the cross compiler environment in the Ubuntu 22.04. 

I also has been tested on Windows 11 environment ( only desktop kits, not include RZG2L tool kits).

Please follow the steps in this repo, 

https://github.com/yourskc/q563_coffee

## 2. Build 

In the Qt Creator, open and browse to the project file "moil_coffee.pro", 
Ctrl-B to build with RZG2L kits
settings. 
The result executable file moil_coffee should be at the build-moil_coffee-xxx folder.   

You can also build this project with desktop kits settings first, and run it on your desktop for a check. 

## 3. Run

Copy the executable file to RZ/G2L using scp command, for example 
( replace them with your ip and username instead)

on the RZ/G2L
> scp skc@192.168.0.105:/home/skc/reneses_test/moil_coffee .

or, on the host
> scp moil_coffee root@192.168.0.216:/home/root

then run it on Renesas RZ/G2L

>./moil_coffee

Drag to select from different coffees, adjust the amount of milk and suger, then star brewing a cup of coffee. 


     

