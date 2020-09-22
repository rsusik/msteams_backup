# MS Teams archive tool

This is MS Teams archive tool that saves the conversation of chats and teams.
It is written for archiving the MS Teams chats of Lodz University of Technology, but probably may be easily adapted for other cases.

## Requirements

Following packages are required:
* Python 3
* Selenium
* gecodriver (firefox)

Gecodriver (binary file) should be stored in `/bin` location (for conda it is `/home/[USER]/.conda/envs/[ENV_NAME]/bin`).

When completed there should be a number of files created in `output_path`, including screenshots and texts. The texts require post-processing to look nicely. Nevertheless, may be considered as archive.

The output of the script should look like below (Note that for Teams it only supports the "General" channel):

```
[output_path]
├── chats
│   ├── Adam aaa, Adam aaa, Alicja aaa, Bartosz aaa, ...
│   │   ├── screenshots
│   │   │   ├── 0.png
│   │   │   ├── 1.png
│   │   │   ├── 2.png
│   │   │   ├── ...
│   │   └── txt
│   │       ├── 0.txt
│   │       ├── 1.txt
│   │       ├── 2.txt
│   │       ├── ...
│   ├── ...
│   │   ├── screenshots
│   │   │   ├── 0.png
│   │   │   ├── 1.png
│   │   │   ├── 2.png
│   │   │   └── ...
│   │   └── txt
│   │       ├── 0.txt
│   │       ├── 1.txt
│   │       ├── 2.txt
│   │       └── ...
├── teams
│   ├── 20-2020-ETE2_General
│   │   ├── screenshots
│   │   │   ├── 0.png
│   │   │   ├── 1.png
│   │   │   ├── 2.png
│   │   │   ├── ...
│   │   └── txt
│   │       ├── 0.txt
│   │       ├── 1.txt
│   │       ├── 2.txt
│   │       ├── ...
│   ├── 20-2020-SMPD-01_General
│   │   ├── screenshots
│   │   │   └── 0.png
│   │   └── txt
│   │       └── 0.txt
│   ├── ...

```

*Note: This script is not supported and may not work in future.*
