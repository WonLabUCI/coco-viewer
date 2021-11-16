# COCO Viewer

Simple COCO Objects Viewer in Tkinter. Allows quick viewing on local machine.

![Example images](assets/img1.png)

## Requirements
`python3` `PIL`

## Installation

```
git clone https://github.com/trsvchn/coco-viewer.git
```

## Usage

```bash
Create designated folder (imageDataset)
Move images and json file to designated subfolders folder (/annotations /images)
JSON annotation file (instances.json) located in imageDataset/annotations
Raw image files located in imageDataset/images

To run cocoviewer, navigate to coco-viewer-main folder
With the above file formatting, run the following code including the path to the designated folder
python cocoviewer.py -i /pathto/imageDataset/images -a /pathto/imageDataset/annotations/instances.json

To generate instance-wise color masks, hover over the "view" drop down menu, and select "Objects" under coloring.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
usage: cocoviewer.py [-h] [-i PATH] [-a PATH]


View images with bboxes from the COCO dataset

optional arguments:
  -h, --help                    show this help message and exit
  -i PATH, --images PATH        path to images folder
  -a PATH, --annotations PATH   path to annotations json file
```

## Example:

```bash
python cocoviewer.py -i coco/images/val/val2017 -a coco/annotations/val/instances_val2017.json
```
