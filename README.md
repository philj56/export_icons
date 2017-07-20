unity\_icon\_export
============

## Introduction

`unity_icon_export` is a fork of [export_icons](https://github.com/ksoichiro/export_icons), 
using [Inkscape](http://inkscape.org/) to export icons for [Unity](https://unity3d.com).

Execute

    unity_icon_export -i Icon.svg -o output

and the several sizes of icon are created like the following:

    output/Android/192.png
    output/Android/144.png
    output/Android/96.png
    :
    output/iOS/180.png
    output/iOS/167.png
    :

## Requirements

* Inkscape 0.48.2 or later

## Supported files

### Input

SVG file created by Inkscape(*.svg).  
Recommended page size is 1024x1024px.

### Output

#### For Android

Following files will be generated.

* `192.png` (192x192px)
* `144.png` (144x144px)
* `96.png` (96x96px)
* `72.png` (72x72px)
* `48.png` (48x48px)
* `36.png` (36x36px)

#### For iOS

Following files will be generated.

* `180.png` (180x180px)
* `167.png` (167x167px)
* `152.png` (152x152px)
* `144.png` (144x144px)
* `120.png` (120x120px)
* `114.png` (114x114px)
* `76.png` (76x76px)
* `72.png` (72x72px)
* `57.png` (57x57px)
* `120.png` (120x120px)
* `80.png` (80x80px)
* `40.png` (40x40px)
* `87.png` (87x87px)
* `58.png` (58x58px)
* `29.png` (29x29px)

## Install

Put the file `unity_icon_export` somewhere in your path.

## Usage

    export_icons -i INPUT_FILE -o OUTPUT_DIR [-f] [-t OS_TYPE] [-v] [-p PATH_TO_INKSCAPE]

`-i INPUT_FILE`

Input Inkscape file.  
Required.

`-o OUTPUT_DIR`

Directory to locate output files.  
Required.  
This directory will be automatically created.

`-f`

Optional.   
If set, overwrite existing output directories(`OUTPUT_DIR/Android`, `OUTPUT_DIR/iOS`, `OUTPUT_DIR/Standalone`).  
Otherwise, skip if there are any existing output directories.

`-t OS_TYPE`

Specifies target mobile OS. Optional.  
Valid values are `Android`, `iOS`, `Standalone` and `All`.  
Default is `All`.

`-v`

Enable verbose output.
