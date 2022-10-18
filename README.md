<h1 align="center">
fun code run it.exe Decompiled
</h1>

<p align="center"> 
  <kbd>
<img src="https://cdn.discordapp.com/attachments/954077931360124939/1031804014339305472/funcoderunit_lol.jpg">
  </kbd>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/language-c++-blue">
  <img src="https://img.shields.io/badge/using-ida-yellow">
</p>
<h3 align="center">
A trollware by my friend, but I decompiled it
</h3>

## Info
* Filename: fun code run it.exe
* By: [mintttt131v2](https://www.roblox.com/users/1775143982/profile)
* Decompiler: GNU C++ (mingw)
* SHA256: ```4B57103C56ED307DA3D78E96FC9DA3C42F54E82865A4375F77850BAD4B2DD4F9```
* SHA1: ```2EF23759BBC71E480BBF9497F98677AD82A3CF43```
* MD5: ```71DFCF127556A4F5F8B78EC5BE707743```
* CRC32: ```EE0E476B```

## Tools used:
* IDA Pro 7.7.220118 with Hex-Rays Decompiler 7.5.0.200728
* Notepad++ 8.4.4
* Shadow Defender 1.5.0.726
* Code::Block 20.03

## How it work
* Starting with ```int i, n;```
* ```i``` is for ```for``` loop, ```n``` is for input
* Ask for input: ```"You want to play the game?[yes = 1, no = 0]"```
* Even you choose 1, 0 or something else, watch this: ```n = 1;```
* ```"Glad you said yes"``` you know :)
* Open 14 times [rick roll link](https://www.youtube.com/watch?v=oHg5SJYRHA0), by using ```ShellExecute``` from ```windows.h```
```cpp
for ( i = 0; i <= 14; i++ )
        ShellExecute(NULL, "open", "https://www.youtube.com/watch?v=oHg5SJYRHA0", NULL, NULL, SW_SHOWNORMAL);
```
* Bonus - on IDA (C to C++ so you can understand):
```cpp
for ( i = 0; i <= 0xE; ++i )
        ShellExecuteA(0, "open", "https://www.youtube.com/watch?v=oHg5SJYRHA0", 0, 0, 1);
```

## Optimizing for my friend
* You don't need ```int i``` as first, when in ```for``` loop, you can ```int i``` it
* You also can use ```system()``` instead of ```ShellExecute```
```cpp
for ( int i = 0; i <= 14; i++ )
        system("start https://www.youtube.com/watch?v=oHg5SJYRHA0"); // I think this doesn't work :/
```
* And if you don't want to get caught, use [UPX](https://upx.github.io/) or [Log0](https://github.com/Log0-git)'s nightmare: ZProtect

## Run the code
* I recommend using Dev-Cpp to run it. Or Code::Block if you want.


## Why?
- Because my friend still think I'm a dumb guy, so I did it.

## You can use my code, but remember:
<p align="center">
    <img src="https://media.discordapp.net/attachments/954077931360124939/1018386384345649172/i_did.png">
</p>
