# Portrait Renamer
A simple command line portrait renaming tool. Batch renames bitmap files to fit the format required by the game.

### Versions

This program requires .NET runtime. If you don't want to install it download the **self contained** release (SC).

### How to use:

```
.\IE-EE-PortraitRenamer.exe [PORTRAIT_FOLDER_PATH]
.\IE-EE-PortraitRenamer.exe [PORTRAIT_FOLDER_PATH] --prefix [PREFIX]
.\IE-EE-PortraitRenamer.exe [PORTRAIT_FOLDER_PATH] --random-rename
```

Using no prefix will result in raw numeric names. It is optional, for example when renaming male fighter portraits passing MFTR as a prefix will result in the following names:

```
MFTR1.bmp
MFTR2.bmp
MFTR3.bmp
MFTR4.bmp
MFTR5.bmp
...
MFTR11.bmp
MFTR12.bmp
MFTR13.bmp
MFTR14.bmp
MFTR15.bmp
...
```

If any file eg. `MFTR11.bmp` already exists an exception will be thrown. In this case run the program with the `--random-rename` switch first.
