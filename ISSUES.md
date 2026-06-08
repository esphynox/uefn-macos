# Known Issues

## URC shows "Validation failed" in UEFN editor

UEFN uses a Rust QUIC library (Quinn) for its revision control transport. Wine's `ws2_32.dll` returns errors for socket options Quinn requires during UDP setup — Quinn treats these as fatal and aborts before connecting.

Fix: The community [source patch](https://github.com/griffi-gh/wine-uefn/blob/master/stub-ecn.patch) requires recompiling Wine — which does not work with CrossOver. The equivalent fix can be applied as a binary patch directly to CrossOver's `ws2_32.dll` — locating the broken handler code and overwriting it with bytes that return success instead.

## I cannot open my Verse code from UEFN

Currently, Windows version of VS Code does not work under CrossOver, so what can you do is install VS Code for macOS, and install "Syntax Support for Verse" plugin for it and open it at path: 

`~/Library/Application%20Support/CrossOver/Bottles/UEFN/drive_c/FortniteProjects/<your_projects_folder>/`
  
## URC integration does not work in UEFN

1. Open "CrossOver"
1. Select "UEFN" bottle
1. In right panel select "Run Command"
1. In "Running" row put "cmd.exe"
1. Press "Run"
1. Enter in "cmd.exe": `set PATH=%PATH%;C:\Program Files\Fortnite\FortniteGame\Binaries\Win64`
1. You can use URC CLI now
  
## Content Browser hangs on browsing props

Unfortunately I did not found direct solution for this issue yet. Only thing I can suggest is browse props via Fortnite client running on your device and paste assets from there. 
