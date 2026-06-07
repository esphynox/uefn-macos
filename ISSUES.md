# Known Issues

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
