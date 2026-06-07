# Installation

## Pre-requisites

### Software

1. macOS Sonoma (or higher)
1. [Heroic Launcher](https://heroicgameslauncher.com/)
1. [Codeweaver's Crossover](https://www.codeweavers.com/crossover) (you can download trial, to see if performance is good enough for you)

## Set up Crossover bottle

1. Install Crossover
2. Create Win10-x64 bottle called "UEFN" (name is important, since it will be used in next steps
1. In right panel "Advanced settings" section enable following flags:
  - D3DMetal - On
  - Msync - On
  - High Resolution mode - On

## Installing Heroic and UEFN

1. Install [Heroic](https://heroicgameslauncher.com/) app
1. Run Heroic app
1. Authenticate with your Epic credentials.
1. Go to "Library" section.
1. Press download icon on "Fortnite":
1. In installation pop-up select folliwng options:
    1. In "Platform Version to Install" picker in the bottom of screen choose "Windows" option.
    1. In "Wine version" picker "Crossover - <your version>".
    1. In "CrossOver Bottle" textfield put "UEFN"
    1. In "Select Install Path" press button to select path, then go and select path `~/Library/Application Support/CrossOver/Bottles/UEFN/drive_c/Program Files`
    1. Press "Install"
    1. In "Anticheat Broken / Denied" popup press "Yes, I understand"
1. Installation will begin and will take sometime depending on your network connection.
1. When installtion is done you 

## Adding UEFN to bottle

1. Open Crossover app
1. Select "UEFN" bottle
1. Press "Run Command"
1. Folder view should open and you need to go to: `C:\Program Files\Fortnite\FortniteGame\Binaries\Win64` and select `UnrealEditorFortnite-Win64-Shipping.exe`
1. Press "Save Command as a Launcher" 
1. "UnrealEditorFortnite" should appear in your bottle

## Running UEFN first time

1. Run UEFN through "UnrealEditorFortnite" icon in "UEFN" bottle
1. Wait till UEFN opens "Project Browser"
1. Important! When you syncing your project or creating new project, make sure your path does not contain spaces. I have my projects in "C:\FortniteProjects" folder.
